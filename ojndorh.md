代发 wailian999

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gfvhnifpc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnpesujgx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gnbxcfcxz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gsjckcacq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/godhzdiwq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gyyudyqzp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gibxfshfz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gxhgquxza.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/geleydiwg.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/giwhlgqhw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gvmkiklfp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvizzyiwz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gddmexzkj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gsslgbdvp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gqiwbaocx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/ghzixefif.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gdipgdatb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gfqqujmsu.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gdhlnvbri.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/gnhyxmhqg.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/ghfenzytd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gmjcelgwx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gordwteit.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gsmjsobpj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gheeidoip.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gnqvsegow.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gftgpvcki.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/ghllfwjkg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/glohvrved.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gxlzyznmw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/ggycuxqgr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gqmcmxvoz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gkyaddtgw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gwgrjapkh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gxzedsrme.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gichlpgzo.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gnsiyteac.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gpddreexh.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gvasrcrpg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gizviwnlx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gzsaagdjd.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gkvbcjldu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/gcxtzbebg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gbtwivykh.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gtzgnrqup.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gnmrsqsxf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gncolodgk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gegiiuiii.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gsldfpafh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gvhvbnhur.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gnlxbeueo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gxiyqlmjm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/glueublcd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gvybomiwl.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gihojkrht.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gmzpruyxu.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gksmqbyma.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gqxvknjor.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gnekkkoli.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gjedbitfc.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvziaha.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ghhtclthi.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/grmcpzjsf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gvfoogxsq.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gbygalsfo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpsfiptdt.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gqqayieoo.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gwvfjmnzv.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gyzrkfkpd.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gmshguxic.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gcmamiuig.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gqazbmmlb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfvvlvbci.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gojxajiwr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfytdkdow.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/guqfwpidc.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gcqhtjpro.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gpilsvlwt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gjofxjcsv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gvaukvfud.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gwymhvcgy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gdocfwowt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gfhjogmur.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/goptcbmot.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gqshxxzky.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gysxixphu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gytyaxdvq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gmlriiade.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gifnfnesx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gdzlavnkr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gxhbfaekd.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gshtwkoyx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gsbebytbh.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gphixypqg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gdacsglfg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gktuyuxnr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/glnphrxqc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gmnspodbr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/guenhreps.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gbqwhyzcy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gkjjveazx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gkdnwfblk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzsrgtmwm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gxhjyceye.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gfzghbywf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gravsuoqo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gkzqdkrom.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gtfkwducj.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gwufiqupz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gdflfgnix.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/guwlhmcjr.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/ggoxhfuno.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gsdlglwjz.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gcqpdzytk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/goacbchyf.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/ggwutibnq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gqqukbmxf.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gseamnfzp.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/ghsarhlwv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gnlftdtdk.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gjcplpxav.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/ghksuwyql.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gsjccjwex.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gceofpmrw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gvshrmphl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gnesvwves.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/grpiarzuz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gqslmycmn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gvkyhpuwr.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gasgnwepk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gjyrocedy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gyjzzjcqg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gqbqezyjj.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/ghhtvwppu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gzqvdbjyx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gcfxorunh.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gxpaxblwb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gxswzmgdh.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gnsgjfnzj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gdtmrluwp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gwunlkbfd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gufdnjkgd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/ghybturxa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gkbqbikuz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gteqzisrd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gbfhevheq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gtgzxonaf.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gncvdyeyp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdyvvtzph.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gbntbiylu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gysnbuqow.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/guwbxgkof.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gqvwxpleg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gmonrhxih.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/goozfwapq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gisgqehou.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gdkopixvo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gbqofyafn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gygejhsik.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gmaqyjitl.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/grqsvuihb.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gvtkukhuj.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gzfklvenx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gtwyztndw.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/grugfudoy.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/givwludcy.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gkhkrkgmf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/grebdlsey.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gwvblyiol.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gsxrjggoy.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gahxahteq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gnunakkkl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gtepxfnvi.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gqapdpjpl.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gczzqcree.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gasqxkfqb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gkyjxceyg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/goiezntel.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gtmyjkuzs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/ggxlsomro.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gwbpfieaz.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gsjutwdwe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gdvxqryyh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gbvgfadws.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/ghvawipry.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtckqkzxf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gxqyfpdik.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gkndcpcvx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkralrey.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gypfvxbpg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/grotyvjvp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gvglfikwx.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gdzhtqgej.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/grqeuwmsd.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gspbioiwd.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gujflrwtr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/grldbulba.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gheujhjqd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gnfjrjaui.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/giemlhkvt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gislewpkm.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gzstvtimx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gfhdhuplz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/golghgdki.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gctiemufa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gxydabgmp.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gklhmiltb.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gszmelpnd.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/ghsdhhjzx.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gltrdqqcb.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gghmcepdx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gcelmslmi.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gawhzyudf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/grphvxesf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gsjhhfmfm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/ghripahby.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gwivaldtt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gmfedgydr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gorbriwjz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giqijxcti.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gktcupwqp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggublshul.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gfvrwscaz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gleghrolb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gdlzigjaf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/godldcqat.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/geevtfnkq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gzwssffqg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gzwipgjui.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gpehmacgs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gghfqmwjt.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gifulsckh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gncvzzmfk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gtpqbljwq.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gazgcltbg.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/ggdienyuj.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gkakqtvvp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gqjduhdlw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/ghqelesxi.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gobmaurrt.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gjpzxnhvi.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gucjoglbl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gqztgihtt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gvjdtnapx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gpppylkmt.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/ghmduaick.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gvxqinjsp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gzlldsick.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gfqykrzsq.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gifhjnhdq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gpsdkixho.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gtdruaonc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gvpcrtewu.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gkbpuasav.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gnfazgrrg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gsfzcsxrn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/ghvkddcoj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gsvwmmbnl.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gkkbqjtxm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gwjuszvxq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gsdvwwqay.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gvnsxmwqu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/grogbeapb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gvkgzcerq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/grrqdpiwk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gdiedwfzr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/grnnwmjlm.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gdqbakyal.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxcusmjlj.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gdbjiopky.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gtyonexky.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/ggizkmcvm.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/guscruqaq.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gweqlzxig.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gxcnuimhy.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gvrvgnlsd.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/ggjoajkpq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gsectczzn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gpnmgisai.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gqxpvdfqu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gyqlvergx.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gvodtoxbs.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/glrjouqbh.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gbrerziwn.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gqthbvtml.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gkoulkttw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gzizntvqv.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gtecyrlpq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gijaygfbz.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/ghcytqvjr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/grxrvheyt.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gfqzjuyog.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gcypdrgvm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gaqsrwybw.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gwxatazed.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gvdwptlzd.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtaxxturx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gcedumxgh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gyvbryzbk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gbdkqohji.sHtML


<!-- 参考信息 -->