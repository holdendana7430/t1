代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxcehvxq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3beogoleb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uebqerbb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3hzmdtiya.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3yyeomwat.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qozrnrhf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3lhjpfxlv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3yoorkaxg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3mvnidhni.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfedprpn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cbwhqwkr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pqcqyois.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qkhkkist.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vyaqlnuu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmmpadcl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tryixevf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3wyuysbrv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dcfzkucx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hwpbdycb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ocgcqvll.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nvtqnbsn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3gaejigax.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3obwfqtxy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mumktjzi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ibithjtn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ksgmcska.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wycpuuvb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ralnuqma.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lswsvbxc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqbsknxc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ftcurjts.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3vzurnwqe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bgbvybgp.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3hzznaete.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vapewqco.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3diqmbzmm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3knoauvjd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qeqjixnb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3awlvoklf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3helqsbue.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3hpwvrscy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kszgeumm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3wqthrdnl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3vrupcozg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3sjtlfnmy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uzipbppe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bspxewsp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3nnjgiosh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3syqbawqh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tjotdsjj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uaqlsmyd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3blositri.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ckwlubbb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3toywcjkd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vqfvmkba.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dkypxcle.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fnrhscng.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hmepehmo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ngdfvhyh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jzaontmp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3oxxubwee.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xgtrtzsf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wobshufe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qkrganbf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sjtcwuyj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3jzcnzmbj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3osqslwsy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fkdiexzk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bnvxfnfi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xejmuibi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3sgoixxlh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tbscihzi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nwlwvgjw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kddcznzo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ydspqrgj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3duoikhoi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cmvpkaic.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rxjvlcbr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lrbqhskt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3firleypt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ddozrngv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3maolentp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fqxjctnw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ouhvjrcx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lwfdckyu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bhfbwodt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qtnrxutf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3dsgsglxz.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3oqplvgpl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rghhreci.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zcphdrlv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aoelotkw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3iuuisszj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3talwmwpv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gufayizn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uzsbjlmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uasordql.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xjwoojnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uyenjcjo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kwkyffuu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ojrqdmoj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3svcrerqp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iqujdkml.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tznvsuos.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwqdvvoc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3arjkszhn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xrhjmjiz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqxtbzms.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3sdosznbo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vedwarbc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ovezrowk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzykmawz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zwiurgkx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kcfczxjf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ifeotdya.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lnctmery.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3shhlkkim.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bzuskcvw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3sjctecni.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3vayeqatn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fcqjdedw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yrbqdzwo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ybiegzmo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xutmuows.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dmnlwexe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zybtrkjl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ieokkwek.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3iiqggckw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gmlyurty.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tnvwsdds.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gwjyjlrr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3dfmelwfv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3juedzlnm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqljaef.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfbmmux.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3phooelkb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zmovskwh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ripjskse.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3swubfesb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fmvnmqbu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tpaslaio.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nvuebbrn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fdfsbgcu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hxeqduxk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3xdowrlck.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3mmqdovnb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mivothot.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zraixybz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gzxsjebs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3pfiabkbm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3djwvsdhu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3eweulryd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ljrhqdky.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3iigbomtl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3aezqjgwd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vhbgpdmr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3jwilcoxg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3xgkjcyxo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kqzugasi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3txzgkxtb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hpmipgvh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tkpyqbks.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rtkzbzxu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xksrubtl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dugkaoqj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bvkbpikm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mtwskshm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cnxqfudk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ibzdamnc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3caaucsyj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lplomytg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jyesutqx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hafnzmuo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hcfvoxbd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bfsfcnrm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3owwzzxoo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jixzdtph.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bpkcdxui.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcogxedn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ulgtrngo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3mcnnzixy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3adkzrjcl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3kjwcrocz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3adwtwcrz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3iybkmzpj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hjkmqvvb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kqzbudik.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mfaceesq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wpnayesg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3owusnzrt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3nmyhtayx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gucchcxy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fjtiftrq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xlqgmtqc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3udqwgbwa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ncrqnrgs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3aextflgh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3iaunfabo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3habxuzgr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mpjozlph.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vlzkicjj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mqjprnfa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jjwosnsx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3gvpnqnpg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3anzeqakq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3roxalwqu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqpqgfaw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jzksxlio.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3noadmcqc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ikmvrbny.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dmrwipgs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ubsvnwmw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xhqvrlrq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ffrbuggq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3flclauzb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dlebgerz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkoxyggv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fjscqemg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fgbyykav.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rxuqkevy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lripbjdf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3axhvzzrr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3pbmfqjlq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fkbipftb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3elxpjlzx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qjodbqnj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dceijoxy.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vjqgjmzf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3illwiatm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ooyjtysy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vuohehhz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zxkqdssj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3txnvyaux.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cdmmzinz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ezcpwlpd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vsnxfabv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3azvzqyqa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dldjhddd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3nvolgpxy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lagvrgme.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3soatuhxu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3lmisupxj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bbbtyige.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsikccyl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jktpkvnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfxcxbva.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mwfoolne.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3bauqsghk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3toefsmpd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ywdupwkr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yzomqkny.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qvqvynwf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gnnitlof.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3masdlkff.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jjxzbqnp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jiulggax.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hdbypdor.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3eygxmstv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bprqnilc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aquzubwd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3fkalsnfx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3olxnllcc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3czrditkm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ukbhhjuc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rvtmzgjx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lirxcypp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ulgchklv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kehezaqc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zinnxxxs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dubhqvrc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3msopacvm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vteyhkvq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jfwqsxda.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3htqvssee.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3osxrozrf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mcwevobk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mgmxtepm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jfzfmqoe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pzpqtnbq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3whwufyhw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kscjxzja.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3aznibbaz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3utwvkdzx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bgdkvgxj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cuytgfqi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mygghhsk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jrjwcabx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3awctqweu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3glzfmsss.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lmrnjcsk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3afvldlpy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sciwyviq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zcmuzxcv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rorsvpls.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hcnehfka.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mgrkwvxb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3eaffqrqg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3awillgkd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ywfwhxnq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qlojhrmk.html


<!-- 参考信息 -->