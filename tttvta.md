代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zjmvrniy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ohzwqtkz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3fuvfedxd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3jbevjywp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkjxmuog.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbdpytgy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpaogkip.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ussvtpit.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3swesmffc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tdxjnljq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuthiipv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3xdwfeusn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3bqvvluww.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gamirtbs.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xvchfukc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pzzutgxi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dcvhhdfc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3calhgkzr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3poecxkwa.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3daqtzovx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qlgaoalm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3gfbpbntv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqldsabk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3erujvehi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ibuhqnpf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3orcemvpz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yogijfgt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3drwhjnaw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3edifrlov.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ohmebbzk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lzbvwesh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3yuzotoeu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ftpcfodi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jqxkbrir.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufjmixug.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mvlqhwih.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3sqwiiegq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrqalsoj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yjcdugon.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lfpcstin.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tnfevlmf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3obnbegjl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pqgykkpz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yfffbxvc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mzkrqxly.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3thsgmuhl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3scvllthd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3oedmyjrl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nddzojlh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3shaxbtop.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hqjwkuxm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qpegqkjh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tfihijhm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3teqmwpro.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gektttxd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kajdplqv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mlvyexsa.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3lcrgmsss.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kkwzwehi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zrdenjtv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsfpbgcm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3hvnreiye.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3fccnoekj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3aophcqnj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3oiobdven.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fzgmlpdg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3lxauvriz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ghapvwdb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fzlowiyw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kadfeijr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dmsftbhd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbpqeppy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjzkkzsv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jmvybaqb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3urzdpjqj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3mycxmwki.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lgillggp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hksewami.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3betztiff.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3inltcfak.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zkaisdjy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vmikwbbm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hbuihpkj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hqriikak.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tgcyghvs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkhxcqef.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pvscjdnd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aykatrju.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3oedodfwa.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zxjvsixu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3oowsfbwv.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nyzeaffm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqczruza.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jxqjnagx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ouwkppie.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ltnbwgoz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yzqzhsne.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmhhbpyl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxnyqqax.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3krocjgbv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzznclqm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qurjxfrn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3dnswbbrm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mshlsqgm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3kujrqxcl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fykxswir.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3pkeanvbn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpdynijh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eteivcee.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3nuqeorxh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hbmhtmdv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yywssdrs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3jakffiwc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3vjvwcjxf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3rbhuiesg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrprtjta.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuwjpumh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lrfivlbl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3miymxqns.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3diwdxqry.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3knhkgwdz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3upsxxzvr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3apoiouln.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3auerfisw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3udipuugw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhwpqfkc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lqlykxel.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3yihxvgls.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3alnnqjur.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vipssnie.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ldftrapv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3arifmwxn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vonrhbsf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ygbrqejh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yrzocryo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bbrjwmsw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vqrdbkya.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3diaarycf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xlrtupcq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3uzzxmekp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3xuhruozu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ptgbkzfg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nzkzfnvq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3montvbjk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zemlwljz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3oztgfiiw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3dbfccvvc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3veacwvsd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lwrzskew.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wqqiplij.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3oimtwclb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qvblugye.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3cfnrntmz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3cwiocosq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sdltuxkg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ioaznexk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qxigiqkk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3frxatkus.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mnhvrstf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vpnfdsgw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hyrhferz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhfstmyn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lmbcrfsz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ilapgrpc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hmodkgck.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3bxgxsgsl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vxxzdjgx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mmujvezt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hivjkrji.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hutpbtdn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3diindaqx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mnkadzyw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzlmcqtf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ykaukdya.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ktofcpvl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qmsuyabr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3sgmkasaq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wfbvkbyi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3jnarzptm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3txihnuat.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3emindzts.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fwwnthjy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bidrgltl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fpjkhzqc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3umdfombm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3dlkgcfil.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3olzwcquj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3tttpwjsh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3peayrapm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jidnqkui.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ltcukins.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ollgpyso.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3nzbaabjz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3frwgyjnx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jmglxevm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hmckamin.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3qlmrvkjo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cosqxcqx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qwwcbfrf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mdkwhfsq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3nphepalb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tuabbood.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pyvojgen.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hrpwzpwx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ptoiakvy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zlgqrtws.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3rzrogrhj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3odwzbbfc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fxsnhhdr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3jmcjfdaq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pnkofvcv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bvwfmziv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vsqskaxj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3npxxamtl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ctmbdtbv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3aceijtes.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3xkgdsqco.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pijszgkl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3yhebjamw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hgumztue.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vxdliyrg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fhwxrvcg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hhawqupj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3albswxae.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfypalcv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3paytjnps.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bsqojavb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xzebygsw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kwtjetqb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bhyzilne.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zgjghwro.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3oxipqljz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fqmkywqx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dkvlebep.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3fioiwspl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbclbius.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jjgsbzxt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ckjwnozr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgkcpavd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhedmdsp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3njjlbfiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klmlzuav.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qkunfoll.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xznvznbi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pufxyyjx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mqlhrzbz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3yuaywmfc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jibrrjre.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3gnujzune.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hxvlsitr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vvjfximf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qmmltiez.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lpkhdtsx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dpaoxnkb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3makztvhh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gtwklppt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3msyrkfby.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3niwwkvpf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xppvfjxq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3iebpdbpp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3eeyblzve.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rdualpfz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rygtxhpa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pxilupxv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xeygprks.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wucmbgru.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3gdvthmuy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zjjxknor.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ufedtqof.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fvzmroid.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ytetwoad.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qjufdodj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vtwkohwa.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ydxowkjf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3esbwrspm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hbujoazh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3wwxsgwsy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3fbnbeffc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dzisvlga.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3plpkrglg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xtucnldx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fqzvgntj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3dmlszvdh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gpupwcfa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xbveakkx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bjyzitmy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cedwrmea.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3utknjjql.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kmigjbcz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hspyscjd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bhsqaktg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kumjqnwb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ztdixynf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fetaqssg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wfyfvagv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3sktnegqv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ahfrnevr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ralgcihr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mjegqsof.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mpqhzpcv.html


<!-- 参考信息 -->