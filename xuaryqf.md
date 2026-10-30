代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gxdrqynas.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gnqfbjljm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/grakyxkim.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gyhmyvyut.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gmpbwhxyi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gslhmixts.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gbukbhyft.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gzmokgkaq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gfanobwkr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gkozfgpqf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/greylcbxd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gwlsfxnhj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gdqgegnih.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gxeowxizl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gpiwicghi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/glqwuacvv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gqfsyzbho.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gtpzkwmvw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gfohfjtnj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gnbvvkvdl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gltyvmtbb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gnvyckpih.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gtwordkrv.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gsfexbgst.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gvemncxnm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gwagwfvzf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/goeminafw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gahimkmwz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gnvlaagce.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gmmtekjbp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/grarxaops.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gewuuhkkb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gzekmopep.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.zdbjq.cn/Article/details/gpxchzzmp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/genvhgiuq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gakjankqp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gmievhcqf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gdchhjiad.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gblkdxwrr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.zdbjq.cn/Article/details/gpolbuqmd.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/giqqskskg.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gddbigubf.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gchbshysm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvsqgcpiv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gakimwnou.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gcjqfsogv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gismqyfio.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gzkzumxqy.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gpzrymkqk.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gnswghzyp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gzvidvbni.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gthbkzbwo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gugwrmxju.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaocflach.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/grljhhjwp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gkglutxvk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/ggzizpiat.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gedvvqhdt.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/ghefpqifr.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gdehnlotv.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gssvtkqsh.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gipuhlzmt.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmslqkakp.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gbripdiim.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gmbmurfzu.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gxhrhjkuu.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/geuthuovf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gfgoirgev.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gionhcxql.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/grvjprhpy.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gvojffxvv.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gpeortfaw.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gfokqfzhp.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/glnlvlxfd.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gqcwjrxms.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gowgwtdmz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmkjfdiqk.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gfcetrlhw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghddgcgcm.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gtktolzoz.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gyszzgfwn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gshbreems.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gxtvmcxdk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gozvbtisk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gjtouczfg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gsjpsqvrc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gocynczfe.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gemjvudex.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gliamhiyn.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gnaynjfqr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gllgqddet.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gszqdwrvi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gonhuiirk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gjtawwsra.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gkoddpllr.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gbpbmbwek.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/ggbgbybbd.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gassgyxra.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gfxfglztj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gnsrjfeuj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gxeorvfmi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gqakwbils.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gipvikrsf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/giwempxis.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggmvskhvh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gxyeivnpv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzpjvnvku.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gygosbvxd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gtpeorwvv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbdnigqlf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/goalfjofb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gmutsexaj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gsebujnhu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/globfgakl.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/grdojwlfc.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gcljokkdw.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gykblanjy.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gdezpfovr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/ggforktfx.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/ggxkjpmkt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gcsutvzct.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gwijuepoz.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/ghirxrxav.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gxkiwisur.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gnhhdsawc.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gkfhwsbcu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gmhgtrfdf.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gehpwfhww.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gxdzslpsv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gwosmwhcj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gcpxrcakv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gudvzzxad.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gwodspdfw.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gjadajokb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gxnnhcvnx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/goovglpql.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gavpzjong.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gkdyjhaxp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gavnyephl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gextyiqnh.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gfngukfay.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gjvgsmsvw.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gcgamrbrs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/geltencty.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gsodpreqd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/grkolupgx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gqtbqeirj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gtazdsnbz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gbnlwlvjg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gcupxgstk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gecuqtswi.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gsnzqveit.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gzxgzdnae.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gfxvfdgks.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gehsadkvl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/graxghggi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gttksxaln.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gutttdxgd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjkwlycpe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gavasybkj.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gxnxepnkr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gmopsfizf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gjduqaiim.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gwjsxfwjd.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gpuyhgdjh.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gjkgnbusr.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gkksdbmtb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/glnxmbqww.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gxejknrkf.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gxhqcvhzr.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gmqqgiasg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gfmojhlhk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gozriqxdi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gpcozcwzp.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/glygkfaph.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/ghjctdkua.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gygbrzggh.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gwmqpfufu.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gkmjfzqfv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gpclnhdga.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/guulsbmpl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/ggxectezx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gmteiwonq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gpleyildk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gczwkcdng.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/ggqzyezvq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/goaidbjyc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gvcpkfhcl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/ghvtoqwmn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gtevqxszy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gatzkcgmo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqhzfmfhc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqqztghks.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gpimozwql.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gfvmyiyas.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/ggmlmxtag.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gxncdxxkg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gnyvwwuoq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gociarufw.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gspfhdslm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/ghjseamfv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gexdoapek.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gclrambmb.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gbeoivbhl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gekvcgtui.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gwrlnrgzi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gghyaukfj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gqveggswb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/glclvunka.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfweuvheq.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gijfgxhke.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gplxxxbhh.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gbgasqyms.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gcvxwfjzz.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gjktvrkjl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/ggftdpgvp.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gxgvurjpd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gjgktbjzu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/ghxnhhxsh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gfimdxfbp.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gthmoyjrr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/grfpgeeiy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gbkxhrzvu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghfmjyocv.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/grqyiednk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbtfhzdrj.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gmhanlfgq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gnmoozmoi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gfpljqjkh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gfddhopuf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/greejnwac.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gnnezrvpi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gwkhbvift.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/ghwgeowtn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/giwenqbhj.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gbcikizhm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gusoqzoeu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/guwmsfwar.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gsloeydwr.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gjdusixwu.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gihgcgqao.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gkfpxgdpu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/guidokmik.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gzazutkqd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/ghxlzkeec.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnvmwjrkr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gqwzrcsqz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/ggqkpakzq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gzywdqfze.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gnfucfbun.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/glcjisacl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/guiktvdth.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gjqqhzmqg.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gcwyriars.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gbhivbcui.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gampzyrkd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gfssbdxmw.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gxjtjfzap.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gdlexnqhz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gurdpxibi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gmaeullew.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gioinhphm.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gygeqqnao.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gshsqauwo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/ggmjjdhqt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gchlosegn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/growvypmh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gzqmevunt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gxvhzlgxt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtfzveooe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ghebgarzr.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gczgtagtp.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxosbdrbu.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gyhndmnin.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gnnwpfndi.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gjmfpnrmm.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gvoyvkqea.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyafpqvgj.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gosamsxmh.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gestddjaj.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gkkwyzece.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gonhvsbmq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvczygepu.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gfareqpqo.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gystsfdah.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gzkithmzn.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gcgjfmzsc.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gieyzgpng.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdvumzt.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/ggqqebzzn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnbkqapf.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gkzggopwn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gdfsggdnw.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gehknllgw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gghuviwxr.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/glsoizvpg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gdlqsdmkv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gvbvyfbgr.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gitlwtkrv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gtxdsaoyw.sHtML


<!-- 参考信息 -->