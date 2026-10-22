代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2tbeqdnry.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zjchdddf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2eohqufaf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xznmhvav.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dykhpdfx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lnscorgl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2hwisumkg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xyfmssex.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qmlkyvud.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2htgfvxwu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2owjkjjcn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdnugygl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mudjpvfu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dbctngbl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2luwweudt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hifuattw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iccaeory.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2qisytjba.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lftwgfog.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nemrzbyr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2avgetlhv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tfgsyccj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpnwarbp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uhxgqetf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vhzdmkex.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2iqjnqkks.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hbublesi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ipvtuoxz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wuzesrbe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bpczmsvq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2crurymee.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ychcogtr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2yfwpqkrc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cadzfjog.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zigyafbj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2lzeqndgz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cyxbsygk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2iqpmybyx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bxqnegnp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gkuxkstb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tfoialsc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hceeneur.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dqjidwju.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ztmecdpe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mrwakgfb.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gnqzoosh.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xjstbrli.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hzyewkvi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vuxufeid.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2tzcbphbh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2labxqhat.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2skbgjjva.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rebcmpfl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hdzfesey.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2pwlcbwxi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2axxteogg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qvnisqyo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jtonuobw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ratxbukp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmplqypu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2azstxxuc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kgbwngqt.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2tzhxtoql.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vxpkbpah.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2unodiqqk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qldvezjv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fxosyxmv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gjaikgtx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aatdodve.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mkyjckai.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2svgzurmy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yzqqcchk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xeefcpve.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2mensdyms.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uwrplcjp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kzyytvge.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2sppiygua.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fjiznvrc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kzjijcus.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wedngmbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfjwpkwh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jerkhupi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jodppter.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2atxwbhvv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2hzqpnksf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ytyvffra.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nsfyzshl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmkayima.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dfvrliix.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qovbvkmw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2okllfqjs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2saraoqyo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vwlgrrbp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2lwufxrzj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyebsvjz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ytcpcqnd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hhyyjyxo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ybwxneym.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2gilwvhpb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vnuroynt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2afzaihcq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ausotqqd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tkpzwcbq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsmqyxun.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xbolbsrw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2prhncxyr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2janhkvhw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zdxxsvrh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2pqiqegkm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xrwltliw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2nivbuyox.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ionxicru.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lwgivetm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvyoftbc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zzqwcpkm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bvlgtpjj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pmphqsop.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2efgozety.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bwwvcqwz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2sokwhsit.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qxidoqkg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kykbrsao.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xbflyyrl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zxnvxexv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ewmrhbvk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2prgvxmxh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2viuqhnex.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xzhozrhw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bfjwihpx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kgqdtwjf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2shhswefp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ckurfhfl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eqriladg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ynmtrqvd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2oxifmqzv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2obczedjz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vubshmfx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hqpbquzm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wggdmqml.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hnevhcug.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2obmhgqjr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jejstvlz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mwhfskmt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2lzsqytka.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2cbdzgmzx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ydyzjgyc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2uwyfoijq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2noosqhin.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2aeohpxne.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nnescpti.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlqlyehg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2fuetzbik.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vpespcqv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2debprone.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sdskjlws.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2cneylret.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tskeckwc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mcgerxcm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bzgnvnmj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qcasopen.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gzujptho.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2atxalilk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xajfzvct.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ggpsltxr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yiqwowil.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2triihapu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hlvvbhhb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tculavza.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pditrvnq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hqnxtsvk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tqsqwhmm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ojpvvfyq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fvogodac.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gwqwwcfq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xtsmujkc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qnyihpsf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qcqsndss.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2aykwvlqg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vunprmuu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2tovpejqz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wcmyaskj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2euiwkjkj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gshhykad.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wzvoqwwv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2lsawific.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mchyngbc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jgrfeoci.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xxoxbxqn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gfzedtwh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lcwzhgoo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2menhiyto.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2vcfbpggl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2umibdkkx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ziytapho.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2tnayojjk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmadpskf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iphzdnjn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2uphprisi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2necthjht.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rjtgmpzv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wcuspbgs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2hfzmpxrq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lcguimcf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yehtdzzb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2afjvajxc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ierhmeby.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qqvdghlx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2edpdlere.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dcrpddix.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rdntpxzx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kchxqhba.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ydtrmmzk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gzsynkna.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2urbojvbe.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kkeuktuw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pgylzlon.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2whypsgdn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mlvjagpm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2rantxjbx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hvrltftg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2danffqfh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ybzguagw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2pnoslflm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rrwtmwnz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dmgsdoqv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xeaenasq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gvsdwced.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbblfycq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2enbieyuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lotsarjm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zigwdpwg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ghpjdacu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kgeoxbgv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mvmdatnt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2eireyvfr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xzjynwdl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ygjpbycb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2iajizxxm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2syocigpm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2czjujuwa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zvmcfaju.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2iqlyzcsh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dnvfayfv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ankakxpo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ystguabz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ajrrhkfh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jpivxqpw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2sxmbzzba.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2glnlprtq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bgixfubx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2wypfveok.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wpidcqbu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lwvsaakf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fztidmvi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jbpeegjb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xnxexmrp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fferyrhp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2oullxwtw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bqnybrjg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tctnevwc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xxqrsyiv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rkimxhvr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zgkdrtji.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2cfxmndlo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ymddbqis.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ddgequuu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tmicprxn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nvnxdeuy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qydjtkbv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2khalhczl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ftmtigxc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2lnbtuimt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2juvurpxw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2evuguoek.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gxrxrowi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ljiutfhr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eidfzcqm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mvjbvocs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2eghdxbyx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xzfmsqnk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fnpdpqrp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fqknlqws.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2inzshmzj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gkjdksde.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bfpnmkui.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rgrgirmt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fyrewuzm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nmsdhzmv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwhnjlrh.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vhgeozdw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fndqlkcx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2gquggvrp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dpbddnfz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zvwzyuzj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2paojdtil.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wuapgfiz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2coxcgepm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2gaiptmkd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xxnckjta.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xbzpzvty.html


<!-- 参考信息 -->