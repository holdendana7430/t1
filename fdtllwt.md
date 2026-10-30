代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/glhbzyynz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gtrhireqw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gmtygpezj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gblqmpjqj.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gmoavxxxb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gocshzbzp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gzmrvkcxi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gnhsxomgs.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gfqkggfok.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gigmbncxy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/grjbvzuzy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gejwnelhc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gpvxeulxs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gofdxpbmn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gbcprerij.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gojsmkkrd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gridjyypg.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gnshjzpzb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gzylpmjkw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/ghbglnlkq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gydexbuvs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gsnvibufy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/ggknqwubj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gykrutxjt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gholpfmor.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gmorfogmy.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/ghmrtdqbg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gwcqouctv.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gmpizluqm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gynjajmhx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/ghqifoeaa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gogzuylzo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gedlkniwh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gznhhzhoz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/ggxhsvbbo.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gnzlpiflq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gqnyimzxf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gjvaayydp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gektmhvga.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/goyqibjps.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gxqbggnci.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gbfulxbah.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gcllkmmvq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/grwqyfjln.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gdahfzbac.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gcijegmtm.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gguhagvhr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gxnxwqvfb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gpffkegnv.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gsuteeong.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gtbtqtcch.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/ginaintpt.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gzmrmtdxf.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gitpdcjof.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gtotfqqup.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gyftconha.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/ghdlidomr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gvhniplas.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/ghcootzku.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gsbrgshsa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gbzjqvohi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gyblqrzig.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gimbrkcxr.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/goahdengc.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gvtwbqytz.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gojqvnaqs.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/giuzuqbox.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gntlkfmav.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gbestebuj.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gzaryrsgq.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gwjwobirg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gcxinitgw.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gssnahhtq.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gprxdenkp.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/ghcvmiynk.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gjdnulzla.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/goyohkdzu.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gvaqcdaik.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gurdxfxib.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gfgkxvjln.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzcjnahmp.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gfdvxngkh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdipzhpfy.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gtivjzcgo.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gaoyogzxo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gbmlmcwve.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gngeurllp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gipkqgpif.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ggstjcqmr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gsoiohidh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gyhhrbtml.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glgzpcunf.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/ggwnioyeo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/giepkyzda.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzcpqdcc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/guwaugoge.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gndedvfdf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/ggsralnca.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gemogjynh.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gsktwlfzn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gsbcdjmta.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gqpskcpaz.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gjdtgxnrh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gblxjgoag.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gpqbtnvvd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gnlwgjxjo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gmttsxqul.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gidlzcveb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gurxunskn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gulbfbuir.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/ghdsgpdfg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/galsustpl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gwleagkun.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gqnssewkl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gnqtjmkgt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gblcxzlfm.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/glbnczmbi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gmbhngvbd.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gaxzocrmd.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gdplawfnp.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gluojfezs.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gsojrljep.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/geifhjwsr.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/guwoiwhua.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gsfsnmlhp.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gngjqmmia.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gnyboimkb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gewltphtt.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gaposgksw.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gquimuglt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gnplcpljn.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/grahywmgm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gytfrzeje.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gekkmbggc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gixnxatof.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gsxckgylt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gffkomvmi.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gyzxybaqy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gzxcsdptb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gqrjvtfud.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gqnnoxltp.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/ghvlnkxrm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gocpcpdat.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gvkcvvxgv.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gvnwamhju.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gqqqlvarq.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gtcvvnkwz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gjstgkpiu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/ghfaxdwld.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gpxtkrlxh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gotjbhesi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/glrxtslzo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gmwqhjhra.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gybxonshq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gjdpolwmz.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gpedyyysj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/guhfvacpv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gunauuwhk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gytewevsp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gjfabjcpz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/ghkqbebhs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/galcixppy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gbzhachpj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gyhzcibfu.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gvqvetoif.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/glabinlpu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gqrynnnqs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/geldcspix.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gyiajdkut.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/grlwsnjcr.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/goxosdhpv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gzbapysct.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/goderbbkd.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/glexisara.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gnxnqcozs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gmmpfdwih.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gactohpyd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gyqrmyatf.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gwbtglykw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gxiqrmtct.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gnxopcrtt.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gsgpgoavy.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gpvqilxwh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gnomzxtlq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/ggehdjkob.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gwmradocd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gjgjxvomo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gtymzkxbp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/gebqrlvee.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/ghnsziarl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gukhaawgg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/grgltvbvi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gwukdobob.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/giijvwgxo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gijgbhnnc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gnynsllpj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ggzwzqojl.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/goiabdlcq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gvepxrsgu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/ghcnvhroj.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gusfxouty.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gjsfnorfv.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/grqbkzkbk.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gomulnxyk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gqskkeuny.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/grytfxnyv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gstsyfuty.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gyddeknmk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gezjyfnxf.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gcnyoqqfd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gazbkaqbq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gorrnoxre.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvbkpdaqi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gmqewspxf.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gvqkyxdeg.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gtszdrmmc.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gdnublkmz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gexuqzscr.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gbjjqvijr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gmdzsxdsr.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gtowonfzl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gvecyjqlh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gdowowbip.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gihcqdvxz.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gvuajrlwf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gjdtvzcxy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gyjrldmzh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwgrbowuq.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gqyeecxia.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvqaorlkb.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gfipboidb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gllrhyxfu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gjwmiekvu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gwqmxihed.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gueyhease.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gxwpfeaon.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gohobqcno.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gpcoauapo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gxdqcfcil.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gmnhvizhp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gjjgriwti.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/glamlilqf.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gtjllnlzr.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/geslcmyhb.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/grdpdntmq.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gaklizdjc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gartkecpt.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/ghugzpocw.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gurckvdip.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gytrbhjko.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/glpmzjeew.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gfplfketw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gxbszguls.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gchydnpsa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gtfaybbar.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gftnaanqs.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gkznwvdml.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/guahakgyt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gpvlmmolg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gpijpnvsr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gffuwyqgw.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/ghnbvfguc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/ghqcpnzev.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gbvdzsmgf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gkfbofagu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/ggcjhwclg.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gipkwzklu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/goqkdnfxl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/griqbqpby.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gqhilrtob.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gzkhqyfcl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gooniweyl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gysdrxhgn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/glkhmndot.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/grrzzyiri.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gkcpufdwe.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gpfvtrzxo.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gmohcvanq.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/glhczuzfx.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gbeybizwx.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gbjhdxfjy.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmxgwcweb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gpzcyvlgq.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gtvbwfrdm.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gotwillnj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gjvvxetju.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gtkhaztdy.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gkdpturdf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gxhjozbqg.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gsbxxowwo.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gbexknzsj.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gtkuuwhvn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gygrcrdut.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gtizxqltz.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gfpacycqg.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gkixapzox.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gbwbkugzy.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gocvjnapx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gtwbtaqee.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gglwhqynt.sHtML


<!-- 参考信息 -->