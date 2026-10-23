代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dauazukf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfpgchav.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jokmqmbw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3omslrgtg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3zjupblpu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zawbouan.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zakziefa.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dfvaujwk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ibcapoiy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ubpgvfqz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ifzjekds.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3svidvoov.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xaqugscg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3igeihaao.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jxymmkpm.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pxcoynnl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ojvgulvo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jhkhishw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rqnvwjbv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vplxtcsg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zofdmbuq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3uagankic.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rdvqmnuu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpetuiuj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mqktfswg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdakkiuq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3caugbtvc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3equnukdm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jatuedkf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3fprcmzxj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3xknhnkop.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3giwtwiph.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nxjvhyqb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zdukwyfi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbqhnnhz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ygyvywmz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zhnjekcn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tebcgctw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3eyefzmdc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xbylcnid.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dnlxdjfg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3axwxrdko.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3unulhluv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ylmfsxfz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mbhxoxra.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3cbdnvkky.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3omndtayy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ughpznva.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3xblduhhg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3muihouog.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vefgyrmd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bnzashdr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qiuvwoiz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cnsmfqxj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3tkhimqwt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3iaapmwqh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3woyssehp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3csibtkry.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kloogcau.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3buexascl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aebnmkgr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ewchmoge.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3aeholtll.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3mcxtorje.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3bpvsuykb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ppbjdmzf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3sevlkkas.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qosivqrf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zruiehaj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvpxhidh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3crhgjgtf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3awjbzyxi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hyzrndpf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3trslzyht.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3iryieieq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3umeopwps.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ovqvxxyj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ksqaaoph.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3apxwpfwh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3exxqquoo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qfppaclx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rwlyowjv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3evvilyhw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3suvrrxqs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xeuwzrer.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3lkutyvnq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ewsxdwcb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lwcnziiv.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ihimmcwd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3sclckvnl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3htiyqqud.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3unpapxjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohpsgpgl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jeaqihhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdyoyfsu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rnoceyan.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bvjlqeko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjhhbciz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghyzaojx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wgeektnj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhbqirbu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ledswvdt.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3xvnndbwf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3huhutgps.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3slqmcmwc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zkpfbrau.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zlxvrhyw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ckofglcq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vxasyxfc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cpcjhbfs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ylwxaszd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3jnmdzuxu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3notrnttz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tzvikupb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fewkfxdr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3sfsdmkhj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtwizqiz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3caybumna.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfiwhkuz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3yqtjubez.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mdlcylbf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tubtwnnl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujjazbvd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zpfntfnl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ddfupbog.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfktzgpn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kyrtwwam.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3cpeezhhp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3aknxexxr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvhnzzo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxxivwvm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qfttdrvy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bryugfkc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3wrbikktr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rcefwunu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vkzfkitp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3bvhqzzns.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3msrriogi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vgbrjqbr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ttsnlhmb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3aqgwcxnm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dmrjycbn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rljigtlq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uumbdbww.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ioipbose.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3uexozghn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pxuvwwun.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wcsdxmam.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lzvfoxed.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3sadsoikf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3jzecfoss.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bocbivou.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3byhxytgw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3oyyvhchf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pftbrgrv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zmgjiyel.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3apqfvstr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3upzvlopr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rmbxpbnn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xxquviof.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cmvufpkc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3phpqtzkq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zstqqpfm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3cczdralo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3acnvcuyb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vqsjmzkx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3efoizwuf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3edptipjw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wnvikide.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tjossboc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ydyhwuif.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3btjbljlv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3apwfrsdc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ozsahkfi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3inmfemga.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lvdhcqww.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3khltwwba.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3zzuamuql.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ajcmvvsz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dxgdgcdp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kbldpuak.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ihzbemms.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mpkktohd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rqjocche.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wyxdinvu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3sfhnriou.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rgeeijtp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mgpriazm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pjxundkb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lltjtdsh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nvfuybkh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3osupjtgh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qmnesdsy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ynyzbzpl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fdlwfghn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3clmixozo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3axvhtauo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xwjyynox.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3abulwwjy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3pfsdoqor.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3izryjbwe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3psxdqhdm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qtpwqyrr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xvjvcjan.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xazoequy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpmmxgtw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3cixavslv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3thrpmnbc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdedowdx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3seynhpnr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3iibnulnl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3iamjspva.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3sqfgmgmj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qsqiaboe.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kwcidzfz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vjovmcah.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkydnqoi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bymdnozb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xgwopvxr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gfdeozoc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ttxcocne.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3msyivcor.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gjwjrevk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qnfaeogy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djaxnhgs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pflxyfdx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qomvhxsn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bitepyfu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rukcucgu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ywtxigsp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3npchiglg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3etapnscz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3usunfzsb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3xwzapmic.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3aowregul.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjgyhobz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3reatodod.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3nkpkkbfh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3crrkfysz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3haqhexlh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3gcoswrpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svwahnpj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kxnpxyaf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xivszmqz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hvaqlpdh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cboujzfs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3pqrgwlhu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3iuwlxmiz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3tasddnsd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3qimzincg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yovtvsio.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hagksxpv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3oukcikom.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3frsxkeku.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gtvdrxnr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fnqrmhuz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hqggirsc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tenzdrug.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3avftpfqu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fvjrtvnv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jsdasrxq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dpjgqxmh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3phgfpldn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kenvazvm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lkbjhrgw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3punjbogg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xmhxtqps.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ohllvfxc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gvaiyscr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nvprujrr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dmgyxnmc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3soagupdd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bfxzofwq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3nvtonqxg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lcukishk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jambwwkz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3puxunqwn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qssfqafd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kkplahla.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fqejfnft.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wthhuhur.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3moxglhiy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ubxkaukq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hxrgtcux.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aoinlwrk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3siqdbowj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lkicsozf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3owlnxjso.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tsyipstt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijgidorz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ojljxfln.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dyjoixmx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3fpfkkjxi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fkmuhhsc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ijfpvteq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nmvdgmjr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vnqfaorw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3yeostckq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hkzsjmdb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3klczpbsy.html


<!-- 参考信息 -->