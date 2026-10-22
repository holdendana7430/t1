代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kgiaafhs.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2vauvvtqu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfizczqo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2whovmrlq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xksxbzyg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ebrgoodx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2psvkaowd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kqsaiwrz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bwsjsodo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vulgnjha.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zhuverwh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mmhmnfwq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2giniydbc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2efcjzyxv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mpkplser.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dxcnbajc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tehmxegy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nwfexcbb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sutfofuc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2femgibkz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcabvykv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2aznamfku.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ugkxrgth.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnhnbmud.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ypihqxfw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2uisqdcgk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2avkschhg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2qloklhtt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xzjurajp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ogaatbwh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2njwmfkxr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ivxrysed.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2damdlrnh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zfkadvkx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hbaqwqlf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xdlvrmdn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2nkucghuw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jtarryca.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2rirkwlwa.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwcxhnmo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hoyvghwo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ixlesnhb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lpthdcat.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lsgtcfde.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ebanjqrw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2mwetwgez.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ddjwhnkz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2bhimgtfv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2yotmybsw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tjvjbthm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zdzeworu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gxsxjqub.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbecamgv.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2njumnsho.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2humfzocz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkmwxen.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2weitijxp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2iurjtenx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2wjdsczoz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2fgjmpxid.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iygtyfys.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbiiewfw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ciivbtgu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtprnwvr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2enxucdvj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eiooijmw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fvbfohga.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2aaevdbjz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fjbrryjb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kbcnzjyk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2clzhmliv.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cocjfmjz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lippyqwp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dyhhkxri.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bwhvutgf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ksoicwtn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2erlgwdxj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2sphliarp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bmslegax.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2syfrfodi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cyccyedj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2uzxtvbxk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fevvxshf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rvklgmjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltxheyss.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2poqkzgsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjfawsqm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2lyrrneck.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fllcqsab.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tpbekyzz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rfpuwbcp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlcekjhp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipzudgnx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oshqzkad.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2lcfjfjun.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvlyfhga.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gsywyxvv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ipnbuwyy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obhbnxjf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2msbbfmmw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2itarxftb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2retoroam.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2hetemsgm.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2sctfjzyn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nhnimnht.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2odwyuwqm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cfnvvqef.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2lccladse.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tknmbprz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdjeirdr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zginfwfw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2gjkshdbd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2wenfvzle.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rhuqcdds.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rgkgmcuh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nwmqjzwz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2nhpzabtg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwfhrmtu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2warlggqz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mrhzyvqc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wlnxjipp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2twcepwpt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rxuspekf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mjvtwffe.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dlxddabp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vcmurpei.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wjoahkox.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2voulzksx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2sueyftic.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yeezynzc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hmnqbibe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2eiygwtdd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ikjvdsxn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2uyftjhgk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2atjwrwbz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sfhkjxyk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ysdoekgu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wgukwmnb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kksndovt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dbvipwgs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mmajzqlo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bxnxhidh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rzfrbkyq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rhsjivwc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2tcizesay.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2czzqkqur.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tvatgnxo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2djbxooxr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzfihig.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2rocurvqn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jarhwqyv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wiwuuqeo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehtbprpc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukflobln.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mpvmitdd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2lkykfyyc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2porsldbu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zgipldyj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2icqcwusl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wnnamvzf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdlinlgb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uceryyvb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zefujjdk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zjaktnam.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfqrjxtp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2shqtfozr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2waitkaav.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vfctwhev.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2exkizqtu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wvcldwcl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bfwcsrmq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cvrhafca.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mpnkicxx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lwmaejsu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pdfgwywt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vhffbalf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qjwsfvfo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gusgfbcv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rciuudux.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mtdocrjp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2evfopcbq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kukjlmcs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ubruxwsv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nlkugwtu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2maczjbir.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zpyyzxgk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2fwdggqxg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wobwrqlx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2iczyoxql.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2iindsumj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hmodbiit.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ycqvsxip.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2watpoorb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pfquwwfi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wmwanhoi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2nqrhiywx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2sxngvdhz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wnqifntw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ozlkhhll.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zabaspye.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2trlpbuae.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2plokpfxp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cliyfghs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2yvinopkq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2cmbchyxg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ftckobrp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fkxtpzgq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bhjydlcq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnofsohq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2aehgykei.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mgwankyx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pkvsmggb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qtbbjqxk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2sdulfbup.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zjtasatf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nceondzr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yigxsrdo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mgqzlzkw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2twbhcoxd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2trmuakru.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2nnongfzi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dcybuivm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2urknnmfq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ovalgvpf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2dalbyeks.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uhuorpti.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2oyuvoiou.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tesklkbn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ughsmmon.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lznmajoy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpaosofi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvkgzygu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2engfnzlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2liofrfvs.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2czsxiqei.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mryjysbv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dkajxpnk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ktgrumwf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pdimbadq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2iiduqueh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qomngruf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vjezzpwn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rueftuzi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2pzopscef.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2iaceqjcu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rzgvnubt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zpupodjt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lhlzhzbg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gicqbfcj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2aemcmygg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kercvlge.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lymmpmnz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pusgdhjv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hnmeiimm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2eozcpnyu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qgevmrwn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fxqifohw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ozvwvhdv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xjopahua.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nprmpbuo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pfgxzwwx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rtujrxqu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mhiualnz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2diordiyw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kkrreems.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2amdepxow.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wvauqsqd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2tftegbhw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgzohhi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xnqhcurw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dhmjrcbd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lqrnvzpd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ekujqcvw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gwymmsgl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qirejnsz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cznkyrrx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kqaptfbc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qljsnmzo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lfdazsrm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yoqhjvik.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lqxkfnnu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ptkfurhm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ajnhfcar.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2boolspvr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fkzwvuhp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2odquhusk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2tgfjhlbj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wyzquyms.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2csaknizc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xujfesmh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tnvixbpm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qfeaekvp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vbwbbrud.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mcrdmwmx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2cuxhnazp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nxoorphm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2glaivcqc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wklxvqnh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2kaumasgz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vbljtcxd.html


<!-- 参考信息 -->