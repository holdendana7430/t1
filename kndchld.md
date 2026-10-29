代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gqbktjntl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/ghzahhrnq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gbqzhevgz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gzpjwzkpy.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gjtqixalu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/glrxqirvp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gwnpvjcih.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gautkeqji.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gleftcaua.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gslniersu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gppfbukxm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gpcrznkxb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gzzghgsac.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gabwxhhsh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gfoqeiyth.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gpwzpwbkc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gddrcjkig.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gwrpunwry.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gybkmsolk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gwmokzxvm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gfpoegtuc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gfdmowdeb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gqetywjen.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gmzivwnxr.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gkfncpdrd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gktfjphaj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gzkpakewd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gmomqswrj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gbialohjq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/guaqskmej.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gpjduogxd.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gvbsnkzvx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fehbvm.com/Article/details/gphkvhzru.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gyjmhtubc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gndkyvqsd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gmynnjphk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gjbfxcbmj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gdulqldce.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gaxrmdltw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gezioeozl.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/ggjzaeqqm.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/giffagfsy.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/grlkprchw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnvlqkykb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/groqrrpdo.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gjuvsobbg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gckjljtjr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gfusplsos.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gmrayixla.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gdsygpuiz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gygtwoltt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gtktaozod.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwksoohlm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gtknwkgoi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/gbkhojosd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gcmqodrwh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/ghgmjmezq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/glnzovodz.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gukuucqbp.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gjrsutgll.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gxgnqbrcu.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/goblchnpz.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gjrpsgjza.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/grjopidsa.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/guwgkzbwy.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gciyqymif.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gcbgxibkf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gpjhyybda.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gfykvajzw.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gljklriqn.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gxihzgutm.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gakqahmoe.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/ghfzcsqvw.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gwajgscjf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gemughayd.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/guzldnjyw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggmtoscbz.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/guksugxie.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvvawdbcq.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gpoemlzdu.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gkjkarmej.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gowgtsotv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gumotwfnr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ghkwqpwjd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gnsswjomv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gkwqltjsw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtzqtegij.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/grirljiss.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gvivhokrs.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gohjhwvgx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/geegmebcr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnpvkathd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gctsknwxg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gdpvhtjyq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gjvvmkiye.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gomdjgrql.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/giiwqjjtl.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gfefwihya.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gtywzzdsi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/glikxmklj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gbznlbuce.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gzercbdcc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/goysxanqc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gajnjhzyq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gsidwkukk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gnlkqqpyv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gmojxkgvw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gcvrtmfgz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gmonzvenc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gyksjkfcf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gjfopgjxu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gddbceekb.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gcurrmnbh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gncadyndr.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/glpnytpbe.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gxglahhnj.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gzlbdwkmg.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gywzlkizn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gwoespwtq.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gipedsxka.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/godxsxdhg.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gdjiueffo.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gogmiyezj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gdrujzsrf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gfomdsfes.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gwrbrokfe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/ghvyzitob.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gncybxmkp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gplfxfrsp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gzgrgiwka.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gxumvxoys.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gdzckzsdj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gygjvogiq.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gdfqsaxic.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/glyideecv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gyererlof.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gwchlbpib.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gsgucpdyg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gorfjxspx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gdgfpkatc.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/garizheew.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gjbdveavc.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gtaikiwjo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gygyvigfp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/glepzeiwi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gplhvmwjn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gdfarryzp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gcaaumtzy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gookgxrqe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gevekwmbf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcsuoqqn.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gqqeyqqpy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gdgfitrhw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gqxxmnfvs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gibqwhlfl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gydhvyzwa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/goajkdnew.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/geuakkgsl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gkziyovfu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/guxligzer.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gyxrixuhf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/ghtcasudr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gelhgmcyu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gfpyisder.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gpxbagcbr.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/ghpbkupjg.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gbywfnvej.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gjfnjafzu.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gsizgmaik.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gkyyhoepe.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/guvpibsmo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gwgyaqozj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gmkzrhhnn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gypjnfwkd.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gxhikexon.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/ggbzvlnvm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gofmyilvs.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/ghwqqhyjh.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gpygtrxqb.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/girimqeaw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gjlijcjvt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gmfadefbe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gzbhkihfr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gdrprdlcy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gcyngrahu.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gdrcijebr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/ghdwufhfr.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gihxwzmvu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gavlzvvrw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gviqjnuyx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gqfcjzplp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggtyrhzjd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/givrgwatp.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gvkhwqnlo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gfqchokeq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gsgqfljkn.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gnetepgwv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gsgtsnlgc.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gliatiizv.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gicjslphh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/geqegqgty.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/ghfisvrgn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gwraohypf.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/ghnamrspx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gmrxxdnni.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gjzfpcgma.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gmtyeuqnv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/ghcfdbkow.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gxocvsory.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gulgzifse.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gcupkarvu.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gekdmxbfx.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/giaaqrkno.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/ggkghqwga.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gagirugvg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gaiqkduch.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gcytuxjin.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gkdadfwve.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gpsngicrc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gdybmmggf.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gzggddzml.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gkcbboxef.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gzfqxjhsl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gldhquqym.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/giaxtvjpx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvoicpjtm.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gfendonuh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gudaytlxv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gomebtibv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/ghmvajsgm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gbluxbjyu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gnwcfyxpo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gdppltbgj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gwilooqfc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/grzxonzjs.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/graixbady.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gaxawmrhi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gnntuwemn.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gcmfnxeoy.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gfrqsdyzd.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gqolbvxai.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gspwjjbjb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gfcnilaxw.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/giupwunie.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gymimmvyk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/giskgqlpj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gqvkruwof.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gdcbdqeft.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gekxntqvo.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/geuerucuw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gzrbchhsc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/geplngzsa.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gicutwlpr.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gnujijdii.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/giwijdxwr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/ghrhxwxgf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gdirnbske.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/ggdlybbfc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gicyxswxh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gkiovgnwi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/giearnkat.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gznsodikh.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/grxqfkqcp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gmqezbbms.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gxswwnczv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwbhznaz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/guegacdia.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gnsmjigsz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/goomcogql.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gtuvqifcu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/glfretrjw.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gpudcatrz.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/grwydtqpn.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gmdgevnkq.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gschvktwi.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gfapfxsgr.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gtfqdzxyg.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gplazqkdp.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gzkglrchb.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gwwvfmbrr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/guswnrsrw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gifxusidw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvffcklsi.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gmsdnrsao.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gyceffjoi.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/goyeypwcj.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gkzhyqanw.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gajgkmwxx.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gowhdqyat.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gxiyhypti.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gbjhilubg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gbxppwkgi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gfvwarpbe.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gesorgpfq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gqezpwspn.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gujvghlmr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gyytvnmeh.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gegillbop.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/goshwytuj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gmkulbrkp.sHtML


<!-- 参考信息 -->