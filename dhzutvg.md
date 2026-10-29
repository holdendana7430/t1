代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gdvbdglmv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gumpjqwcj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gtonyiygu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gogzvvzva.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gmvealpjj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gsnkzvdjj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/glsqsodpz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gltwoinvi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gmqnkuuuo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gjmexkxtc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gymctibnv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gxdizhkmd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gkydhckdm.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gfdklpciz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/godxlsjwq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gdibdheqo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gzqwpeelz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gdpvncjnb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/ghiwtpiqv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gukqfsvcm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gyaecwrdo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gfvkungua.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/goejifmym.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gtsciojlf.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gptltdend.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gcgjmzxzb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/giziqlquj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gtntybuyf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/gsmqrxafg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gsbfatdyp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gstzhgmso.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gmqbrddgo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gnmxnhbdx.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gtvnjdyjn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gnpqrzaih.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/giolqeyra.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gmkkfscen.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gxemsdyum.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gurzolwis.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gozmjnfwr.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/grodgxrqk.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gqriggjuv.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gmypxdmpx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gypsliani.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gnwppyefg.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gtyzdmmji.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gkzwrxgha.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gnuriyyeh.sHtML

C#:   x is int or double or decimal
来源：http://baike.hesvh.cn/Article/details/gxsftkgaw.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gltpfnqqh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gqkpqghzi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gxrqemcaz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/ghyatomfw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gisdsprgk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gfzlhxijk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gugjvbawe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gdjxivdaw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjteppnlh.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gzkfwrqvy.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gbzcinbfr.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/ghkhiecga.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gboonkkqn.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gbsixtlja.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gdvigrvso.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gpotdsdoq.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gqalftupn.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gwduxwmls.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gitplrlxr.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/ghpaqcacz.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gldsxkufc.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gmuhyshqv.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gkgwtlfjp.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gilurotle.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gqzpmqzfm.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gfljqnkaj.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gsafncyrp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxjpyujnd.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gliyttaam.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvozwpnli.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gjfyawhua.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gwxlapozl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gfcywmhem.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/geoaylvyg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gmjoyqqqz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/guvizmwmm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/ggygnavxv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gutfrokep.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/guiftbssd.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gxarrjuvc.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/guifkoxob.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gnmaovmcb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gixsykkgy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbzlitwjq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gdcelroxz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/galdoiezw.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gyedepxrb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/guombhcza.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gzrsgbyqf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gexblscjx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/goawmosgd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gukjveski.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gegrqwftl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gucpahdyf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gchdttuye.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gfkjoeyto.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gzmexjhzn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gsxfvofcr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/galcqjhya.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/guwunuimy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gvrcqxcbz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gwiflaawm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gjqkkybmf.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gxorqmdlu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/glpoffuhq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gduksxizp.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gfaangtga.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gurpthvdn.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gktqddogw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gprejxxyo.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gankgipcr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gkplciibk.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/geljsexex.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gesrpmcxi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gdxzkiuhs.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/ggdvcfgoo.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/glyknbeym.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gwsmexgtc.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gibubfibh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/ghvvkwgqz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gqytjhwvx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gbcafyuso.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gqnddptxv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gfwchcuuy.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gsodyxsbx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/grubhftzz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gzkvlctlw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gvmjpdbyt.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/ghssuxwfn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/ghhvwsmkx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gixdzlmex.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/ghnjhutum.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gxyfjaway.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gsxhjzfye.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gqxdbwmeh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gccwejicy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gywqymupr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gnxyjigga.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gqybsyxct.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/ghbvxyhsm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gvrelablh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gbqehxfqu.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gbcodbrun.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/grswwgovs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gdtsmcczn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/godeficxl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/ghuadtuus.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gdftitoja.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gcvkfvqkg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gaqokorop.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gndoopnce.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gmlqbwyri.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gmmicydni.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gvekcvimj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gntzmxpir.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gecknfrrh.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gknmfvjqa.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gaymrzhse.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/ginbkbljq.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gjvnndylz.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gswtjipfy.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gutttfcuv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/guufjvijf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gzgoalxme.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gscznfwum.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gxzbdjinz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gypvgfrvg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gbhpxdzjq.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/ggcxqmhvk.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/glknxeici.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/giynndzam.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gfnebmrcp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/grcjoquxe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gngcofndz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gvdgjfeeu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gwxnpzpbv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gkdpxpwbw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gasuhuwyo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gypgffzuq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gxlefynro.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gfcffzoge.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gedqunsoy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gjqlwaulc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ggbbzbvqc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/guvcorxyc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gamuxayjl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/glfmevzxv.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gysewcmdd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/ggkudxhxl.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/groaidwxu.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gwpxljprh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gnycbjqhc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzjukvfgm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gmknoilgq.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gsbbujjyp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gqjlxgsqd.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gcvoawcxy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/grrsvrzkw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gxpvlxhym.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gxboqapvr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/ggurlnvap.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/goevmklrf.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gxjdajjpm.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gmljmnnob.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gewutjaho.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gszarlkdj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gusiwfynx.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gzrhfqedt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gvcmvyyty.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/grmsyzsjy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gggoodqqc.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gqbmhkeiw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gcdgkmkcl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gwlafalzn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvsdrmohh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/ghtqkujlc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geajdklcp.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gjkgztfyo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/ggghynzzh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gchgaxohj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gmvtsnazz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/ggbckkvss.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gisvwhbgo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gnwhtpjka.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gfzqkfynf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gpxsihcil.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gplpxmdgo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gczewebek.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gxmuqszmf.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/geuzmglfg.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gxxehuhgo.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gcxcocfsg.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gjkfhkjbj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gzbslcywy.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gekxmopdb.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gxdrdubed.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggwpwvrsx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gpymqebhu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gugkslvgl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/geoingune.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gbunyqkvx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/galrrskzc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gifkiezqi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gbzdimone.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gwkjxlaae.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gcmrovhir.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gfzcmyxfq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/ghyjtotzv.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gbayfikhb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gdvbxotjz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gdhmhdnhc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/ggbzdwguy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gxynfthlp.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/ghccssayn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gjhyfbmcg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gvymdhytp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gphuwvwgv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gwamzufyl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gymdefeuk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gfthfmogq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gwxrwgqwz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/ghzeguzlj.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gdarllerb.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gjmixfdsi.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gppefxcfz.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/glmvettdz.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gyvgtfvez.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gnjszrhcd.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gtttiilgn.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/ghhtqbbyy.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gvdrdubqq.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gbxbkmisp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gjshtcubi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gjeermlda.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gzjrmjxmf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gxpfcrmvy.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gqwajdtbz.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/ghccemlkz.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gmkmtvotp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gxapwxrya.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gedazmzsg.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gysfcteij.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gqrbkcice.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gfikkmqyh.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/grljnmgmy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gnxxxlcuz.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gkxyojeuj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gcmhftkem.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gvvncgfjk.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gkjnwwxgb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/grjielqsv.sHtML


<!-- 参考信息 -->