代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qxizybse.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdxrvaty.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jghmosgl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cgrrutli.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wqcwslkm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2clqebhpf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysxfwkrm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mpdceqfh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ntoenzhg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yupcbapz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hvjbakyj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tmagidoh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nhgdndcj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vrpsfqpm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jaueulek.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jreyurze.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pjxyhbss.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cdmavglx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlhqmgrh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lptvmpvm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryxzzzgp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2slkntmkg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gtiwhhld.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2lppiqxgc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ccitufgx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2zmbhvhan.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2oaqqkoll.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2kjevnbtf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wexrkdij.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fcibrbyw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2tbwqqvak.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bjekcaes.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hotagylp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2haewqnpc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2jtqvsqem.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2rsfmimoz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2flfbxoll.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tuqsbfdb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2alpfoehs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2exomvgzw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2npvuqnap.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vhkiaafm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bwmbzhiw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2oxuzyaor.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pspuppva.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2hgspcusq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vedjdgki.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pbumwkfn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lzvnnqdu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rweoebyi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2pmhoujdu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2cmalytce.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nwtxsxkq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mfguiatr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xejjregm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xldtnqzv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2secjownx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2hghykfvv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2hbvsdhla.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2laakiwxf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2dobdhnek.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ungbljwe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2uqpzxabx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hmnkuckw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vffiisdv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxcfpmkz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvhydcgf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uuhmppse.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2osyvhtnb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vjzmmajs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2lwtpoemk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gfyromrt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2wgfzilgz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aqwsgfoq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ayajnjyd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hqfffsxs.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jbbqatwy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fajsiyqx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nkyizysr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2tylxrnjp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ehmcqxpy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2yafsvnnf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gcujgxdu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cojgyhpa.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cnkemgbs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2grsvaexm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fmwlrpzd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zysyqndx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kuhukeqd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aandmhrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugomumsi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jhufgfkq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ayhjhwfa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjgwbpfi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsoetjjl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xqebmhvz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yhmglmhk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eaxvlhcm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2hcybcdct.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2czyulfeu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2usoxomhi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2moyecabq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2bdmpimnj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hooujbhm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sktslvmw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2pwwjozih.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wiwekmkt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ndphamgx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zgeqsvpj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2talupnbn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2uoamxlza.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mqhavnys.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hjpubjjf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kioyszgv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2erhajhyw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2stsqlhah.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2mcwgcbch.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pzzuiedk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2xfwmnayc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2oebqwajg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2xvyyhvoa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgpxlkco.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dlldwzdj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dbbjpyms.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dkgkobzv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2apimwbgh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ggntlpjk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jocnhfqa.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2efsxyxye.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2usksfdjo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fkeamcya.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2oqzmxbec.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yvawbrzx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uswtjaxf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hcrqnrzp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kibqdeny.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wbnrzuqd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2lumjrukw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ivoeblgu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2knofrzrk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ywqawils.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uyamprup.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2oqntwkwu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qkkogdus.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ndbycnyd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2hlajbtnp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nwdnlhvg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zobdegve.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2pwnsdnof.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2sinvneak.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rscnkfsj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rmttqkvg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tlfnzbvg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hhownfma.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2quupkrez.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2oceyqurs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcntqbej.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoyhjrix.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mhrmgihy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2qvhbupck.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2gmofoluj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mllsausc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gzwctquf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ghgcrlkp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bmgixyje.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tpbtkihb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bszbxbmm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tcyqzbql.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gfbinyhz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2sdbbrcgm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ssbxjzhy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mvopguxk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ryhpobvj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ydaaxlse.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jcqupsdf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2udopwndj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yvvfnzyd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vvqbhgwu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dpmlhlmy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2agnegipx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cgbabjns.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pqgttsbj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gmrnkgpf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ubdcwevg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cvolkubn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2traspxxq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hnttiefy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vcblyrpj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lwxqbens.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2booitqye.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pwjirjsc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2uhouorxm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2klnvuduh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mapiyyqn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ngefiowp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jieicrdo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qzarbyzb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2sgkiuncl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2bdyxzsys.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fxpwalif.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jvnjtmmb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzkrwmqd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fuxaohzo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2awemzqxn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czifyhhr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nsiaipdu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2spgsbvhb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2lkjrzfsa.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2vwrlahaa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2oayieswk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2phkebmto.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hdvdyytn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2teqbzwfz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2voxwyauo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2iztndcth.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xgnhsegl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2cxxdnyvg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qrzvorej.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qvyyikky.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qjvrppyd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ruumnozv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hiesndsw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sfdtnlba.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2odzjtecs.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hgltecux.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2njfjfoas.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lidllhhe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xkmzskgb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rzuxtiyu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lpmkapaq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bkgxulxd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vissgson.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cqwwkssi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2wkdgenxs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rzhfcgda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yskubltw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qceubrqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czgdbelm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qrzcmhgi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2wwmqguab.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2geckfuqr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kaowckkr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2yygodgxx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ghelwztt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xxfpbwow.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gkfyncip.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2irhoiiqe.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vrwobrjg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yavmsjxh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2exdkgptw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uqvrsqhz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qwuqnsyp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xbnjkejm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mvtipwfm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2icfiyxdu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2foaamglp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xkelqtjx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2njjlolun.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2niigweud.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2cnngqtqs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kuuvxojx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uewextvy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zmkxkwoc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2uvsuzfje.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lmephhmt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2smdeumdf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cyumckny.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xizvqjks.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hoyneczm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ivqpxory.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2chuzeuwm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2iapovvgh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqnhsmze.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bddzagql.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dnaiuxwd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2knqtcuwk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wxozcavv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2btdcbsyi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lofmjfcf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2asgkubvu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iasvbxzy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hkhgnzqz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2itwasfqe.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2imjxhxjw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xysejazu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hpxkgkaw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gfvrqzyv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2syzzitxv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rbyfqzeu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbsmdczt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kdjsmpct.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ttwmotpu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ietsajdy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ixvksttf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2filnmolh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lzhetvaf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ekxefjam.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2scrkofbp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jjlicshp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vtjdemcm.html


<!-- 参考信息 -->