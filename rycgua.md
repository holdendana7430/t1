代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ojipeapa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dfdhsyxd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2tsnmmjnv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2llgqiovj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2xvgayrkb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mzjqdcpm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tjqjlnfq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2auhzgted.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dkkvbrqq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2drkpwola.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqmkqfxm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mgwamcbb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2nakxwlin.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fdfgpskn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qblbqext.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lvzkmaki.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hvnsrzty.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jntidfhx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2yoonnqur.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mxpipqqk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2aindhoen.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rdaycgku.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mdyfwzzk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wnhklrlq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlorqvms.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtpmpyje.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2duxmxqsi.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2uyqwoayd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ythnxomh.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2echbalqv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zvwbeosj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohbowldp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2maufvyrl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cdngobqh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mhewvmnb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rgpylpsn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2btzfzslx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hscoswem.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rumebqew.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ucoqjxwc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2livyrgtt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2quixvtjx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xzlwxuex.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mjvnvsmt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fysqrmxm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ejnhytwu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2rrbyvlux.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fqojuljp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mmjgyzmw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2xnaamysw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2avkvebpk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2foshatol.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qizngtyi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2oothojum.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dsbqbtiz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gkifogzg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2avzxgana.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ghknwlud.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzfvkjde.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2icjzmevq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gyyvmzbl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qmdvqotu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bajobbmz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2gwssnunu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rmswogzp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ryvtscpc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2kgsuqpxx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hycsamgx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkyocerk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uucvopfi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bvglesef.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lfkkbwnb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xqrbueed.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zwcfjpzg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xutfkggu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2riypffpu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2kqilfnfa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jkoltrox.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eahqalvb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iqzcazad.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pwsejwcs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2buatsclw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ovixpawp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pskotdcc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2gqzzafno.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hsiyauzn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gfozfjxy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qdnfparj.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tflnkzrm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ukavnlcs.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rkrfwebo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2theqoglr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrqqqpzm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hlglzdai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erdrbjbh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mcyfaccf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rvxgfoic.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddgeitcs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdvlaffu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cfexlxub.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjleezql.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uzdknrzi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ottzieqm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rsghyrgz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hrfydywe.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2axtsgytx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuwzbnyn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojqpadgq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2auzrbikq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2lbmmryqx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dovnwssf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2eemkwpbl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cxcuqnof.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mwgialfo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yjwjuddf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2auazmypz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ltqinkut.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmlrmksw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rnbksihs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2svfkjxur.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2algtkylg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2clwteziz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yhworblq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lqetjkld.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2nbmdurpx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaqkhbsz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ealumupi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2txwyehsj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ntradbef.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rjczhaoc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mpzpegqo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jagiowic.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hmraaiik.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tzoxzxgd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ariylivy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2algoklap.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ypniwvsf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2elwqflvq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bsyawgoh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zmsajdrq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yfavacae.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hbkmggyx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2orcmvlfl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ukykqmkh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qernkfev.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2dpxhskoj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kvitkell.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rbcuizaf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2htrzczjv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2uvjjzbdd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2bexmkhsh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tvypaupx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hqwzdtil.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2atnftuah.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pkezserg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2tjrsxsyt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2nxsafaij.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2swyfaayg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2knfjwfmm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hixilzrl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yufhyzic.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rwavvjta.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbsaxpcb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2szienbmn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yrpiwyoy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wsxoyeat.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eniwjaqr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2yigufhvd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zykttdhl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2chfjgrdt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lbeofzdd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qgacurim.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kpwylhfk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ahlpmyiy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hanynlfk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hmsdqhge.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2gujwlhxn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dnpljtzc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zcfcsnyq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2sgnsbxmi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nwzguepc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cfpllphw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ysuvskdf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zljoombj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ptziijre.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2tphitmwk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gadroode.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2huhtsfax.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2touefzsz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ddpbntbp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ngblmlfb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jgpfxvwm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2kczhjrkf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pioradei.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zqddjlog.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ppiyvmzs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2sttawqiy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ipvrxtst.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hpgerqec.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mskxpnzt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nfwraxvb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nvxrtpqi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xhqkfvoz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cszdwkgd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dfmtzdts.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgqsnish.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ytindqxl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ftsenymr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tnqwpwmq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kcbtklir.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ormlkaxr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2sigyeyoa.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2phutdzhn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xqqgvdlg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2esrzutta.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tljldobw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpnlvadp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdnbudpz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gkabpzqy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uywxagnf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2oaarmgxn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2pzfoyjnw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bqskiwbc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vezpnxpp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fplmkbox.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqqamwhu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hcxqlxna.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zqgnqfoz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jjsrtloy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kfniptkn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ctfxfvxu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2gjezmszb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fvbpllyb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kznsiylp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bekjowbl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2otwyfozp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wdlbizqc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xkfkgcrq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvkmbpib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nximyypc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2blxkzqqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbmbpbnj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2eglamgfo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nrucphde.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fctiuxac.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ehctfedl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fscggqso.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bwmiyrut.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dqeewcjb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2itclhmny.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xjohmdgr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2tvxfgtqm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rgdpzjfu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tgqdutpq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nuqivfmm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fecbdemc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2reskvzrt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2asenfopu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pyhajmbh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2nhlscseu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wreggcar.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zthkrccf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dnkopxsm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ckipsfgr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wxbzezej.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yxwkwdby.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iautlcci.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2eazqewxp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iezoqtgn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mofcqnis.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2iiacdtba.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mayulqfs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yokqitap.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2sqsgcnau.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wimgzvvr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gkfwdeeq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxagwzx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2tffkzauj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2faiypcoz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2txvartdp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2exrsdage.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ceemrliz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2cycgtfey.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wmtctday.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xinbmmsw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rzudhvdr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iocvrkvo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mvfsuhbn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2obywjpeu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dvwvnhzk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gjxjrsiy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kfulhulc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zabpmemu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2idgmuwqz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2omlgojzj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dxecnlad.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ukzbtgif.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zyfcluep.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wjzgnbtp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ttrzgylg.html


<!-- 参考信息 -->