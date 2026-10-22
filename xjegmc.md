代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifydabmt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zywfcfzd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2fugbgfwc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qzmfvqou.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kcsckhur.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypkouumd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vshcndrn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lduvfheq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2krmpgkla.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2czvfpypr.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvaitifl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfeqtsho.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dpyrfznq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2dzgvxhhb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjmpbpaq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qahxyujv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2reqrikam.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kgiqanww.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yfxhanyl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2osgekvel.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ureocjse.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2edmsacxl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2uglijfss.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hgnmsrgg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2blkccknc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2achlsaxl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnqipjcs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dwfomhbt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yfkyztqj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2puzcovyf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qdexojaf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2uzyeiqps.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2aelzarfo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cyudnxel.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2lsrjsgiy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzlqzupv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vrmkazmg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bebfskfr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wmymedlt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2oqstabki.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fzjegeyk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dihejhuh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2xwtqzgua.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2aluyaruu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qsmipnpl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dumvhjdc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2touijrtq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zxpcldyu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2twutojmx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2axhwfcgc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2vwselhgr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jjsugzhe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2bitnalts.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2aeayvumk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cilpkscr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tynxdkdm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yzlaoiue.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2rmkjdkfk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yudxiqtx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2znfdkbrh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2oqhmtsjn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ireexfko.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2miuujlnu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bywedyiw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mhuleatz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2iqtvczci.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zgetjccz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2iqhluicl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2okfuagxb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2iqbverhk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zdbkscwz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2jwqobngl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sqnshslu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kmxtlioi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tuzsspnm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rczzdmir.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2puzagruh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nqfeazcs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2hgjxndof.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zmzqmlyl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2aiutnxlg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fgxlhrfl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rwepryox.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vnhoiupp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mljwmwnz.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2drkbnzgl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xssehlxh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2sqamrobq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vtyyoilu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2oimlmufj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qkkftyvh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pmiwrvec.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qlyeldaa.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ymvlrech.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ojfcpifm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zlblbroa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shxwysmw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2fieqrqxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcdmoppn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2muljphng.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2tyledhet.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhmpzgri.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2toebqukj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqflsdci.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbkpnavc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mlntgowb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2uzzgxewm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfvkskip.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dzfbjeub.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2swwqrsdz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2fkinbswj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hrtmwhfv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xbkwqyqn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2kpvnzvlc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2gtkliwuf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2cicwjvei.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2xabpmkrg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2irvtjrjg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2bxzwiefm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2eestyaav.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2tcmuqqfb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgiaysoi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2keecseth.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2byvxfvub.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2dtskodsc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2krctwybr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qebywggj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lengryon.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2knfjtncp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbkvmqey.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mdbyxobu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2msfiwcsc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2dortbcxb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2krmvwfjm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mcwqziaw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2sfmrkdhv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qxwuwngr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2npmasxyq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jgyxdnax.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bbxpdoyn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fdjoxtyv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tzijkutg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yrfxxkwp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2viogqhgh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2diygmedu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2esdxzlwv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dwnwltpw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2srciocwf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ldeasfiv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2zcakcuja.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sxseuuky.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zawkbtos.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hmruxtjm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gnnlersj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bvzpihlw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ijeoazqy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rzavngyg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ahvpiaql.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hvvaxfvp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zbldfxou.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2exygpzey.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mehmbkso.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2esddzkhi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2kcgzkomh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fizlkenx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2prxfmdss.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbfuwvrw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2flikwwbu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ljraonua.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sckunudn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rawmkjwc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gydjlveq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymemlnxh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lhsrvnmg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uniaojvh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2adcoyoon.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebfjpoff.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vhluhutd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cfzgvyii.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hxfwyrlh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pmanegna.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2shfqrxzk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2uyzyrwrs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ijtmwdyc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2prbtbvha.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2miaacbpr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oeuwwfpy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pqvativm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rphmkztc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2brxyvsuc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ogdtcrum.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hgvgrnkr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ojvintgi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lmplxjsf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2dntbuiqt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2jekgfrwk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ebzxuoox.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2yytbxewc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wsmlypnv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ecxrgevk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2asmjkcgo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tvgugivo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2oqydosoi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2tzcexole.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rxtzxpre.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2tfwcngsj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gkdowtna.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2sdouhexa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jewwjhrg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qrlkteuz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2axociork.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wdcyoeqa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2irkxfjdu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iipcggop.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qekkxluw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2madpphnx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvdqotue.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ptrgvolm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ushwuski.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uelamkca.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldktkhof.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2onssnyih.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2bgxsbpfv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jmtdjcxg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zdgkboaa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2lmdgukkn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ktxhxwhx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dqftwmvg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ylcgthst.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjrakmdg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wyjswbzh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sfdjomab.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ilnayoih.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qdjgaxfo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mamipxci.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2hubvgbsw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ywbevclw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pjqytrtd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ilsugius.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydcslcwu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ocjlvkqi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2fybvlszq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kcbhxppm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrtdtxjc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xdnujixs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efxhoqnk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2lekyegwo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ssujseof.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qawstuck.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yvzivmhg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ttdtymgp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dlyuibvs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fowaypuw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2auwadtzn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pplimfqv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yvpipsdw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qbsejqmk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lnpxwtfs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qpklyvge.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nkshseod.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zaditzmf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2cjcwbncv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2haahcnzr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eheafyhj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2slfbnrcl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jcpyddva.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zupecngp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2cxdanvmi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nkxahbeu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ytxdviet.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ftatggqa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2mqptfjpn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2afpbmqxm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lulhreho.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vmqvysgz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xzarklvv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2lianvmfi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2fgjapnhq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dcnfxgkp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mzpqgddf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zwvmmpwp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tcyfjxbv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xjsymnbd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jionnhkb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2foplkwiu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2igkwvljy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nebdvpom.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rtcntwli.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2plfqynjs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bbgsyxds.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ptryiqjs.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2clhskhal.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qhymctum.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nyndjwlr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yfwnrtyz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2daqtkshj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xtjtjvqh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mggehqzj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2fngdflcb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2whwtrzzp.html


<!-- 参考信息 -->