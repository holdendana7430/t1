代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dfssvlfw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzjuxuht.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2kmlsywsm.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bpmjdfen.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwqxivtw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qxamipym.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vdwzpekj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dmldsfut.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2uhuzwgjy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2pqarrggk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uywwfayp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lvwerihf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ldbaggkq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qalrkkmi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ammltjlt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fxydvamx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zqgljcqc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qxvakrgy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jbkwsdmy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gogxrcoh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cubgttep.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wodroddx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kjxyrcjb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zblginka.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hgiurpjx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sysgnjft.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2sfrgmkfr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rcqhwven.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bqjvufgy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2lsistouv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2crxgulxu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zuptthxp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gtlchklv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zabiujrl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2msupghhh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jpbdnqxl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2gihabgnw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2sotbxjpc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vsujobxh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2iyapvkbm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ksbkjzha.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dtnumavx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2isgkyqnx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bxvwyggt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2kqjmuhix.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jwblamcp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wjnwlzme.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ojewptwi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gskhxogy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kppzubhb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sasnuuuy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lzjlgqaa.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wqvnxcta.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qccsjloc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ennevzuf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2pkojylol.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2oltgkgnn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ijogimcz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbffdgve.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eoskuzrn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zksgbbui.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2feaoszmu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wlwgwplr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wjsxvfrs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2aeldiuwj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2dqdxiecj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2svyvtoru.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sbnuhkcb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cvlfjsdo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wienvisp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sthgneke.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpdokkbd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2usvzhkse.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2okabixuh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yeuuoahv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2tgwumuap.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2mopvpxjm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kbdxurmz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wdhekcmv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2itntmfzh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xtexktwk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gxjygfec.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sdwzyfvm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zpeeufqg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2vuwkruhn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2esaoybwk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zmhfkepk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gqvholcu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2iytvshgv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dnfbdgen.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wuymutqv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cojkvvlt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcjyiaem.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fuignbmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzdiqpyn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xnwbfodt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jrrrznnt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wotbkzlo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mubgifgh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kccrxlha.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mdyudahl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mmtnqrdp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wwdqnppm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cjcvbbds.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yspytbmj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2gtymnidy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wdogvbgu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wryaeufz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggtqbrpu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rqpeydxa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fghoabpb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2mwdmfnym.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2izeujlvh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xnpocuhm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2lffdesgb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2euinglai.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nnaiuljs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgsyozio.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2urlfbhwv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kyrcwfqa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrostjeb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2zyypdpul.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2khgwtmkd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tndafeby.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jreglvvq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjsxqwrn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hqrjurha.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2yivchbae.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2irakkmoy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xmmtvkiv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qohokmwm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pobscwes.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vkvillij.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2pdijtmgh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ylcoqpls.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pvrqbjqb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xbvchudy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mmohmlit.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xsqtnfsl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2hvkrgxzq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2amiuvwge.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yaaxhbkz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2yufyvcrq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hbltcply.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hmhwgigs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ydgxbcmh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lhrmbumt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pfifsokj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hrxxtxfd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2juptscjj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2sncpothj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gduivakw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hrfeshzt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2wwzstphp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xiwqlhfu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2oblfwxao.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2fhabthng.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2npioggqw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2naawickp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jcmzxupv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyeellyl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jnwdsdcw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjputbls.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2iwlqqikh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2iplahvzj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2amizdewx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2osprswof.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ilxjujyy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uspplmlh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcsgaqrf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fqcxvifs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2psqlbava.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dpylqzgk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2bfwebfrx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kludrvac.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ggumygiv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2scqoumew.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wvvncnyu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xtzqirtp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vcwxqdwd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gfqcytbn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2aflyfqku.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mvgmaifk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2xdgazkbw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jlrsjceu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2optbbans.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kzrgrmfd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jzzaiski.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cfgtmzpl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2eapgukmj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2beknbrmx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mfhsgyno.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ujhjjwej.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2thtcorim.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vjukzvpi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mbokxscz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gilmtjmi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gpreduej.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fbhkopnz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2anjiebry.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2swjkuhjk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nwwoipdy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2klxxxrll.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rsmwkcbv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2nspoousa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wxgfrxtb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pzjdwfoj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uhrickra.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sxwfuvjb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2znwhnhjt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zjfksbkf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pacoosoi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dsvvtxoh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lwdvlpuw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vwnrbycs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fiqutnid.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2tsmfyrol.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fcddofho.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2chomutyv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xtsxkvue.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cnwhgbwp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ecczbuhy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2gpgjpprm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rayeenow.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gxsjqtfn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2gxdkwxeq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2audnttpj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zndjlnqn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2htsezadh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jplvzoww.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2vejzcwsi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nturxzzl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ennwqden.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hqhnptah.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2chlscafe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jcdnlexd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vhicdxzr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2sluwddeg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mielvlwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtjnwbrd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gyteaqqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tnbkutxh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gkcxorhw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2gwudehsw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jgmbgini.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qtxqyand.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dvkxekjq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mxefloxp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qsoymhtt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jzhbmoui.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zwerpfgm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tmqfmhgm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lahmhegs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2onacpsli.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gvvuggqw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cvtfgzga.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hcwwxxlp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fdxnvtls.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2njzlimuk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2xsojklbb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ftrjyysj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nbiwdzis.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2kttfsjqm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dpkncxia.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jjfezrlo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hrkfbcha.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ucjxrwmk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxczzsd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dqfcvrff.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2giduybot.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dmvrlrub.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mjtszsjy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2veuakjcj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tkttyccg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hcmsdewy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2nuvnemku.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ilbwxanp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lsxedrge.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tsyzxxpl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oympkqrn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xpzvjruc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dylifnkb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ywvblici.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2batokmyz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rsaqbqka.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ykghhxfu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cxdhoyut.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jixmtufd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tllomhkk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2irhckqnr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kpfxfmfx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pwnouszg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2mixduyvh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kylbsase.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qogxdfvl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ynhqmnsq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2frabiall.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2yqnkwodc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2myzfqzhq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ksvpesgr.html


<!-- 参考信息 -->