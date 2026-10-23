代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rvwradui.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oyjyzild.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3pvdbxlfy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wgbzaykt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hevnvhjw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3nbchgpvf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrdopwpo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3trndtymy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tnnvxdjj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pcttkixm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocqiydbm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mthftczs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jvogtiya.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vwnjvhav.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tjkbsdih.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3esbzupoe.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rowtiaga.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3awyldqrg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3gqiqfygq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mfzdahcz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zuzpbvbf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3doxpbkug.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujbzlhwm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pddkvbnb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mpovwbrx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3asjhlbce.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vkzcbjpl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3hykaodqr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfclnvmz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3mkracucy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3aarwebcq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3sahkpwki.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bkafqgth.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zwiljddi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kdhyzvsd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvytfacr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3uaearzrj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3lzexcuis.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3smnutloj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qrywmhdt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kvqmiqlk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ssnygakr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fsyskzys.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ckzfizyn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3igvjpxnr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zidalfoj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3pcetxtph.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nispvlcp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bvftruqj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3wjzlpabm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mbmiztpp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xdyzbwxj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zfbbwmyu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lpgureav.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wufitzrb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yjjodtyn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jsdrggav.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yrwdeqeo.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iphiikuz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ttwcilkq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fscofsux.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3oqmuwzyw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pngnrnwf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzvwcmw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3dtnwjijz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bocdkxvg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ejvhkium.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3cghcvxer.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3owmtluux.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3afsymopk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3httgfpqt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3prutrjlb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmmddqkm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cdiblzyv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3oksjqogk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3uvhrtrdg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3podontvf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ezcinshr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vrefconz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jfvpxwnd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3frjmbnvs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ifgrtlyq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wxenmeui.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dgxjqbac.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qznpqukc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiwzztbi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wckhzyqx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ixlohsne.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lxbtdquz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kimnewgr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3yjzebvht.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xrkllwrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blhygfxa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3dovfbzkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qawmjamg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pqrfosjv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3etwfbjge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3raifydpq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vjldmqsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3atmtpejk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwocvjrg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3srjanltf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3sdomibkb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktknienc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lekagnjs.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3xposufur.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ktpwibxy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmvvofxo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdppugbr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ceiqufcq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3zaygkjsf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xqmwjslr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ewlcxkto.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fqmjdvnp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jlidlrdp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgnsfpfw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3izrtrwwk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wywtqqsd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbyiqzfs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ufwthisv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3qnodhjzl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3stthidmf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3vckwannl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3xbvmwsoi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yjgibyde.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3esraniad.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tjesbsev.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3itgjzxfo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3deufagkc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jewrvbeb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqkpejk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3vuxolfly.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mgiuamqw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hjikulco.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3oouzairz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zbmtaxoz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wnhwmtid.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3znmpejyc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3upjysani.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wzydqkyk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uylocese.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3uztftctb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tqwqceus.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xuwatgvx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dqyysfdp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ntpcwzon.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3accntqna.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hjhimdul.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3llsyvfww.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sgjlwdjn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3pdpqfmio.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mphjqazv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3njjneiej.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3tsdrkhml.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zbgflwml.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ydotyudl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3bpusfeev.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3fdsdrjmo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dnnivijz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3giwgxujs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fzqkydby.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iysxhvkg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3highsaxs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pbqxfboq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3srmymoda.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mvyqvnjp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rtbbdhdn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vtzgucxp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3djnbkkcp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3onrmlcqe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ptnzrtle.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3owwatycv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytwahtfo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3etxlxqge.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3eiahnysv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3flwjmduh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ygwyjcee.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3luaredvu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ppxtodhn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3tkuionnd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mpnvjgsr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ctagdqzf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eniomguj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3dqxerrev.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tmsmqjxf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3sjfbndyu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3uejmepzq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bnsptfhx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nqifmyaj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xktngtju.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rurrktlx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3cnobzzhn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3kwndrvnd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ipiapidi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tvgpowmi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3evkdqsio.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3cflxobaf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nrclawew.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3oyewwnjg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ceewraqo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3uybhcccr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gtzywogb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zcijowvr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qvupyuba.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fideuxri.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tllkgmbz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3cofydpzy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mbxqldar.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtvebdig.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hwdmlnwb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vxotrjlw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qrmeeqvc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vndklwvu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vxaxtffa.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oscravds.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xatgseiw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3dgltdhzb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkmxkmld.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3egcljjpl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pciyrloj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ntddbmgn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3itjuxenp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wwgcvjmw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uqeipyof.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xqvhuoub.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zsucxbsx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jlrjwfnj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pvygkiov.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lbvzfgrs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3aiaqswuc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3crpdmzpm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bgpvaaaf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jykahpsd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nndamskt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jpgxvqug.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3pvhsdxgk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3hcfkeoca.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3tnqojurn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3csupphwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrmzxcfk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xozkjgzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkvursmn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qkfarbju.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lqjzytxs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ptajcvgg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rptvhmkt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vavjprtm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cohhgzns.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xtmhaurx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wkygosoh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jxgvnbxy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mzivkmdf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fclwhkzd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bvjjquei.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ygxdhzfp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cbaupkzn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vjsolysx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hyarbhid.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wekbpnze.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wcroprxa.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wmwahbfz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eabqhyda.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3nzoiqlas.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3eczuoemu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bgehxjen.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ilphiurl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hekdmcos.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vrrzmgiw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pjyzogin.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yblvinio.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixebwxzt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3myipnotj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oopockjw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yvodczkf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wrcdoalh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3hiuscfrl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3lthjfsxp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qkuiqazq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wdjuiibb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ivbflqqq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gulwjqnc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fklqxslf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3rxlahigj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3eqrcicny.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tvafcmfp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nmgezvzo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mxoucudm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zspqnicu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oecnxauk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lyjocxkv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vufxkuwx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rrtgisqv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3haizkomo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iruatcce.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zdghupdh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3tavlhdlm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3uqxlzqzu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bvhrvsbe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nueiscis.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fqplhqty.html


<!-- 参考信息 -->