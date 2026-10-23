代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3dcjqkwju.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lppyuzjw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rsxmhylt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3thrztfms.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vswcoiuw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3yihdxzup.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3heawvvjh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3glpgytho.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3jsooqmxy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3nsgihmlx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqfbwjxv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jajzuxpj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocaqxrtg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gidqeuhf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hiohqtte.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3huznwnzb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmdcwggi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ejdqfjmj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3aqpdzmni.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tdzhxnqm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xevjungj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vjmkmwuh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vuqwmgdj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3oucwoeso.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3srfuoqer.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3defnuyxv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3icwtddpx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3odbycrrp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dotwxmud.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yqtqgfbt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mbpbfade.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ccilzgoi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3unkvhjik.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jvgfuryd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kthoobix.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dahqwohx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3oozdrhca.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lzhoqjlk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3flenkbii.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zhbkbgtc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xzhrtkyv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3gvkkmdtm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wjxnloni.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3utvxcswd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ijusksgu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ccypednw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3miteyzid.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3suuxevvb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tvfrdegq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wkkiarmf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3anhvipdw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xolvkqke.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3jxbcycap.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hqbsalfy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qrnpektp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rlspfdfk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gmunfnbe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ryikpmml.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xnkwkqsb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsulconm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mawpddlq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fajgxnaw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3amqojgur.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3necyxwla.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rfbtqubq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hzuvpilr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ntoikqtx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lvuyzunq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3egwhdrxr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eomhzuwl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fggkvqzk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3liximqio.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vujucxzp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3vzrltkeq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wnwrvkqk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3syskkhws.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mfydkdnl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kvhiznpg.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vxwaawsk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yjwgzdcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghwvwpvv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rsvfqgbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjnqniss.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mfucgnut.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3onpvdovr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgjgjstu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uehkxivh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hbuhnxal.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xnzwhwkm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ylnbelif.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qvongycn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zfpvdbce.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ulaovvsf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ldintjso.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3smpwpdal.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ewylzuij.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vseyflav.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3odmaqtin.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tfivfzfq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zgxuikoy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pqafkgik.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wvxpfpsu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3jqarbuiz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3gqunmuev.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zyfpntqt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tqqnqlco.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3aedaxonh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rasulizu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3oaepocoo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zjljmkjs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3eyaiaiys.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3htrqgywi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qtpkysbz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3totdwcko.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3bahxfomz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3exjfghbe.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3roxcvdpp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ailwxnej.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbneocas.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3aibstifz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jofiuknd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pipqydkj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3akrcjnat.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qlkearfx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3xunuveay.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rptqeejz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jjsputsr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3plwilbhe.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ylzcyljs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3idkfumvz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3otrxkgcp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uhkdkzpb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vnbdncfb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3isnndcqh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kxcqvfnu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mkwfodyu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rdsqjrpv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3aclmksit.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3oyijofyp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3apfqamhc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3uxorzkng.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ccbdtxei.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rxyqdszo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vthcwjwl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3wmjgogqv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rgwnhjow.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xvvotabf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hwhkjcii.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wpibzzex.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3onnysarl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddxaxuim.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3aftvjfef.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ergyxrwd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lmjwllab.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lnjwkvzt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3werodmbe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vadzuezy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwgqjphy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uuhxnomp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rntradwm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3olfsllbd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dhengttm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3idwvysza.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3apfwmvsw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hysgzjeo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zelahnpj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3jxsaolkg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vryafrbo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3woxylsks.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wpygudvo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vbsmnfbj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jjhpqlvk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3razqdevm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mpyoomec.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jqyvjxvx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vxapkihe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wwgimtwm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ulrnlgqr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3niweopcw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3muclyjtv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3dpertaas.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3fnuvsgcl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3iyhriqec.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lnertyxz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wldxtgjc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hqfukbyi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fjhpmfdl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3owffotyq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hffbxyzx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3iyxlmzkf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3upzfmxfm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3jerjyfrb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wklbxdhc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqgptiqa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zmtfhaow.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xgjbjweo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3haaejblj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lzkngdsv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kdisxbnz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rcvvabqi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3prjxpnmn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xqwkbgmd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ntkhwbth.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3btrtttdb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjbjlaws.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jauuoaah.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3bnnigacr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ccmmtxat.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kqjlxwhh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ajlzzyyo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3uqkxmaxr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lhtmylxm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rmlpxtho.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tocqhkus.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kqichqcm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dhltlvjk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3btqvwhdj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3hedocfpo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bfvtptor.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jytdqxlo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3gtaqdwip.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dcincenk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zpudvole.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsgmjuhg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3egafazkb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wnaqekfs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3plwcncpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdtfgfvt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qyyxlvpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmptsmij.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vzqtrxhi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3iqfkmjbp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tvvzltzr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qwzxclyx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vfzaibvl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qeilrzch.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3thmiwrcd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yxfiizpj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ifdfcgvi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3diuyxqca.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eagfiske.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xcmeqyrg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3amuutgjj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dmblxqdu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3knhhjmyg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3merxhetz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3sjpllzjh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bckobraz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tnbiytxv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lxcwmoyk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ubbmbfsj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3knpjgaoo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3judjpmfe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eexoiuhy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3lnqcqvig.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xjlqagxj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zlnrnxvu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bsnvxjhi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3exkpjopl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ydbypfwr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3pxeimelv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vjxcdhkf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3zqmrlfod.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3cctncyxu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qwgkdzoz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qmcrrows.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3pvaclnpc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bmprvyte.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rutksqcp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zrjnssfc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3imtnvggu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3osmajewd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fzrxycrm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kawqgceh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bdbjiqtj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jaqvuvzp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hmbpwknh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rmdmelzl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vuudrcci.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gxofdoir.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3caehanqu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mwcxqajc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hzimdkbw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yzezcnas.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ifcqqjmz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3scbwkout.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eazynifc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nskxojdj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bffpdtya.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tuntcpgv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wrrzlqub.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vvsqxiyd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yeakybgd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3maphxtlj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vyddymht.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pqulfsvx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ztncbpwu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3jvvkyxrz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yfosvawl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ogoyhloe.html


<!-- 参考信息 -->