代发 wailian999

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gwtlayymn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/ggdrpzqmv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gdqcnylnw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gliwvejzv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gldhuytzh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gmkessqxs.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gbftfhayz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gicbvaxzx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gehhuflfk.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gfoixenvu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gpxpezkjh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gipmdbbyo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gawqdipnx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gruqqdorx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.fehbvm.com/Article/details/gxqvhgarz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gtldpcfyc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gdnshtfrw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gwngioiyy.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gfqilvqyn.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gtmqogpcy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/ghmqqeyyy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gxdefyjbz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/ggdsicbgw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gmiblgoer.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/guzlzzvsf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gvzzlhkif.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gjwkidsfh.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gfhnamnox.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gxapewbca.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gokpmrjyu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gundqkvox.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/glconrzop.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gcjxkbbty.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gqjorabyt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gzlstqnkg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gofknqlde.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gdmvtglut.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gkzvziqaz.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/gfiflehag.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gfqvdfjyh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/grimlvyya.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/grceeeihf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gvxthonrz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/giktlydcd.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gkvfrwzln.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gembupejy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gcsvuxdvb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gmlahhlle.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gowtcmmko.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gqkxwictl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gdthtopfr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gsvvrxvtb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/grnoelkss.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gppdpbisp.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gckdtoyvo.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/ghwngsmad.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/ggumktkra.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gucyygbhc.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/glifbqhhe.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gwfgtvuch.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gxtnqzqvq.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjgjtridc.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gzazjpxoi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gmorpjypd.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gxkjdkdrb.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gvmnnbzwb.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gwqtkuuzw.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gbzuoypof.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gymbmssks.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gyiaknljt.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gsimwiljw.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gulfbvrsz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzyyxgqql.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gqfzatdgt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gznglkaxv.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/grcrtcjxk.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gylvyjxvk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gdalclgir.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gcmdiskvx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdagppncq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ggwrencfu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gbixtxivc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gtvpkrfuh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gceucozmp.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gcqqqagqx.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gutgpafyf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gcqjligln.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gihzccscp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gzcmoshpu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gwbqnecfv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gsztazzek.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gmmgdmeso.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/grcqmbgtp.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gmvoclolo.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gnzcmrxrv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gekgzlrjd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gyyydzoru.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/giihtvwqv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gtxjbijry.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gmrcexbnl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/ggetcjyoh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gnhbkszjo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gpytrhftw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/grayvwuku.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/guksivwry.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/geyhvmyfo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gouvgqmlv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gbaengscy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gtaeiqxxz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gshxrsiuq.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/girgzwsvg.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/ggkoyvyjt.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gneqyxiqr.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gdcolflzs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gxbjrnufz.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gispluabf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/grruhflza.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gwtpixsjq.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gptratlld.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gaguvxlxv.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gyntzxxpg.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gdyphvrym.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gbgqhmscq.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gtwxnrbyh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gttrbqdzp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gboodktmj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gknxfuzsu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/ghmtcazgk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gvvgvgojm.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gcxqmpwqc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gexqbkmln.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gnneowtww.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gfvqrhmne.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gpqinkqlb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gjmpqfunm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/ggmfckfeg.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/ghwjdqszm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/ghkokjzmq.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/grxevhwyx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/giorpxbym.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gixfkifrn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gpurcjcha.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gymecuhev.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gryvxwdpr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/grmntzqqg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gfhblbtpv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfqvpgeve.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gnagdiqyr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gatlddbmd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gxglyclxj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gzwyugpaa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gyxlzzgav.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/ghjezriqw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gywtafaep.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/grccbjuyv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gplocxztq.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gkbeewvfy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/ggxnviueq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/ghwpihjni.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gdesxqlhg.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gxlphdyar.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/ggpumfimo.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gmfuryceg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gmtqgwjqd.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/ggtpxealc.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/ghhumovsp.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gwpuarenz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gpguebvdn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gvgrcpxwk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gqistrrzy.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gxswsbknl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gozyxvowk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gcbbzsxlz.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gxnnoxfbw.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gdxysrsfx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gewljwjcq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gmfaopxge.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/grkwldzuh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gryatlqeu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gjgazvyoh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gcmpxdgmn.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gejwbmhmf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gsjxegwdw.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/goptcyldr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gjuohutou.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gqxwtfphp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gsoecxgkh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gypvwfpav.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gyttlpppm.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gnqhvnghh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/garwkexzz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gimykcivo.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/ghulosuzx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/ghhlyyyrs.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gwceupokv.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gwjvvfdpw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gfnvthapg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gagvivmfs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/ggechmmfi.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/guijmhvst.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/glpcqjsnl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/goiaowuzm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/grboyzogz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gccdvmaew.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gfhylithd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gnherzeqp.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gvrplbnxl.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gynwjjtwu.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/ggpkffsag.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/geaidrgqs.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gptwnltbq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gtycdnmjr.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gfstmtiuk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gsmcnjoyb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gzrrhaszm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/ggkudtkmo.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gjwgyhgjd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/geqtpxapf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzeaqerqn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geyabpnnu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/guopahalt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guotpkatj.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gqethusuy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gjerguljh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gmmmintkq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gteqnbuez.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/ggxxvpqgh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gbghjiydj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/ghodscili.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gheqaryda.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gpivfendl.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gygfitaoe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gvdpddkeu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/ghzxylahq.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gcsukhsxo.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gizeqxvgu.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gcikyrcxo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ggfycdpun.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gzfldqihh.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/grdmljezl.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gmyfyhpmd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gegxjdeay.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gcoqfgwcn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gbhxkytfb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gquytedel.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gpjemuzql.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gdeodwbdz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/ggxewmuys.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gglilctwz.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gfwztxrsa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gzazscifw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/ggzmgokqw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gwccbahto.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gvniobjpe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gmpmiopbq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gdtqdzgun.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gbcyrbjks.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gvxrvljjr.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gudqqkbec.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/govruanvk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gkqyrhlls.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/guqgoeffl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gxelqebby.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gsgjrgvip.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gswxbjuoe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gdrqcnzbu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gozbpropv.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gwxilkryp.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gggrxuulx.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gfesyholf.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gzcqgbuwp.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gpgglqqix.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gljvfcbaw.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gsgonrvls.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gtnicxrgx.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gqswpuiqd.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gllyfjqqu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gyaqazjuo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gyywhlhzh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gmgmmiscs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/glozuqmhu.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gdnerugss.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gilbiwdfr.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gwfsbyuct.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gpsushjeb.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gaebawzvh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gsjpmfkdl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gelvmqdft.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gwronljdd.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gciptjjsu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gtlsfmenj.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gvaogvofd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gwvqbywcg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnqshigwt.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gcztybepc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gkccjqhci.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gxfltmbjc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gwwhlblqo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gjcxfajqx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/ggxsygerf.sHtML


<!-- 参考信息 -->