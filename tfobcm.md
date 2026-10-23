代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hqadtgzj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3taqxiogv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgljrjkg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3qckbnzwq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zwfgdkwa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rjrvpnom.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3cbjrojkq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3iqmjnolt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxsizikh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bmelguom.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3atcgzunx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vumvnvms.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cnsvxbor.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gcvcqtpr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgddjjwv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ooqqnqeq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3poltngly.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bwfybdme.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3keackwzt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ootqembe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pnazkqkw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wwqswrfg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cbrwhmwy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fqzucucf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3oazzhiwl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3luonkton.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3djboddbk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgjjvciv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnvlsrwx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3znypkxbq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yxknrmrl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3jqjhrake.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3njordpaw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xinvizvj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3bwuansrg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtoxptid.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qayxpppv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xbtaalga.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3zoksziop.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3sgtvvryf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3iidqetoy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zzmsqvcz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yinddxkl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3krcyxsqe.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3wqbraoqv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qcfyswbz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ijuhvxol.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sasdlnjk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eavmpbly.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3sfkpndct.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dzlfdqjk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rqybsmhi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3szdropnf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3tokzpdpk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nrgoeydg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lahzicdh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qufsnrip.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3nzmuclxd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ywawpjtd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vfgovvxs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3hczdtsfa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3oosudkvx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ywxskiuj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qqekrhfe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yiqwurdf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ywxtirpc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3twdpdhuz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3lkuwgafp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zhemsxsw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ayaufskj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ktxkfrkv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qdhxacxw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnuwrydz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3elekguzt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lnngphsa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ysgmtgrz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ipejrqzz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ezynzssq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3iijgunat.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hjyqlsno.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fgefqrlt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gppnncip.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ldjxvvxe.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3llrgeqqs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tvqbyewo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ivnnisdh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3soardcjz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rnhitacb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ftjfgtxn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tryewueq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qqolkubq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oyomtfjf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tppqcxao.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3urlgezsl.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ahedgrxj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3npjgjpgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3revhcjhm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3nscaofce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsfcsytu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lhasjyft.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3tzisgstt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fqnmikqw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iybqyjbp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsydckja.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdprqeuv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zbhrncbb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3tzwtyowc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhdjnbai.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dlmxwwoi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jmmzcttx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufovgpih.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcitthet.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tcizalmz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3sxgbzhzx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3gvhcnmoz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qdxtedip.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ohadqkib.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gvbkmyet.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fjldazfw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcqfhnxw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3donpouay.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zkbumvzt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xaqsjiuj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3dvyvfxaa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3rwozmjgl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ummiknvh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3flrzntmg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qxtufjxz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3lkqveczt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwcftuwu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hilqmlwy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uqvxuqto.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3eidzftmo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oybuopor.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jilyperb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3iuuarhrk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mucaytcc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3emssnsad.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3phuumega.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yfjpdscv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kaggjaxs.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hbgvpsds.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3deebrfgf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3epaoatll.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lmqbdiew.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qlpogweg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vcegtdhj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wsnzrpzc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wdfesqrb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3masnfjtf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3oyxqrrkr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dcebucmy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eyrwmwlf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sxrtviuw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3caltayjs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3irfkxfwh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ouidzwhk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bstxuyal.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qxwcwvyv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3anhjpjyk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3aaeuqnow.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vkuofeje.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3iledlksz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mdytjoqd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdrfyezc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3veinjbsq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wfttzmcu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3evlbcrnb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3iotsfhxf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qjlbpgvl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiruwdla.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3sgeymenz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmrkzbfp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xqbkkvmc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3spjrbrvv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rqtcikbm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwncgebm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3yajlvkdi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ervwhspb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3dexhfepl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vzwqrmav.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xfinuijm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xmbqsqjr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vfmnqdbs.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zvlirvig.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hxxrhwty.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hxxgtivp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ncvaubxn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ybrzzwpk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3fxyzqhdf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wdecwmpx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rcbgjfze.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3khhkjrzd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cubgctfq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rmzfhxjy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yenzmofa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jxxxjxlz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3sdlqblit.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3rnudeyse.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3iwlveofi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3oyckumtq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pidavaed.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iesbgmgw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mledrhfa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xozodpnq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3igapaklh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pprojbwd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3sfsdpeim.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mscesqeo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uwujlzlf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3aeazlmfc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tetervxf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gkvmalgd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3edewpwmb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3naikrmlb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3apknkaxv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mbtezfdp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3tdtecect.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3thofzcmc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fvtfiyqo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfuytsoa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vearzcli.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qvurakiw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yqdgnwog.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vlpdviix.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xlqjrtrn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yjxdzsgw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jfmbmjkm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnckovsy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hcazjxak.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xfqtdiip.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ofpcjbae.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ruoazorm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3zvprlmpc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3oyodobdb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rggbooyz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xkemyfno.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ykagiwwf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wvddvcts.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzlgoefz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xepepank.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3fucaccrr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ayoaoxlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3diwzsfco.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dicgpocj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phibcfln.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jyvthpvw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ggazhesh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3glwiicmo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xltnlgbh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ywiiigrp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3hpgbjnvx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ndzjuxnj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ozhphfsr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3xodogzze.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qezrcrvx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3xkfylxmw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vjyinytb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3eeowozry.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ifxxeqtt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wcihksan.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sfjnxvlu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3xqdmyzhp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pklnsdcd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3odsfrgpq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ieskskiw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mqbnnmnx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jigrnbxu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lzhixvbp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3owddegbl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zkovbots.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ylbhgzbl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ibtwplxh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xfguxryn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xufirqja.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hoddbesh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3azaikysl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zuovnnwn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fdstyuna.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3deqednky.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3horejuhp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3uypfdddv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ebnroylq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pjqwcmqf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xnqvbhnd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ynlrljtk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nqwwfscp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ftmtmhvr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lcclulxs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mjfqxxgv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lrfkblkq.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3iyvwgzir.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvfgytoo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3shussvhm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ejlytbgf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3etrgdmto.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cwgdfzgh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkhauro.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3anwjfdzl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3mhahbnks.html


<!-- 参考信息 -->