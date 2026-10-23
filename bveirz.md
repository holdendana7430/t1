代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wxqhhads.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3hlspnhxw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yylgtwmc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3smyitgeq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3awbjbejr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zphrsbkr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3prwfshxk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ncykumjr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fveuopqn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wuavfwle.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3umebmrex.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3goaqohrk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3flxcrqjk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ajlkctfp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3davjlbmm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yclqlrjj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ocxhzwem.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jnbqduge.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fxbbtuyk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3yfyameib.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ibjlueym.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hesdnbgf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wurqpuga.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfghovim.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jdpstogo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3akwdelgm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kjpxkbeg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3gxzetajo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qnpkmcec.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3abnhsmpj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3jxaszgni.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3jxvauhct.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3pmfifhty.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ixfwagpk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vbrvpsrf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tsjdeboy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3wehyczzd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nmgmggrt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nffzifpy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3siqwbift.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3pzeferdy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3emmychyq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3juleiafd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gqapyldh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sjauvvaw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktonfhkg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ybmbqjgp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vfkplmdo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3howccxkc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wuwawasl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3begzpulg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ysfludmw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hcogpzqj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mtrivpnd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hybxyowf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wvkzixtw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3nwrbduuj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3hssmzlmd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3sxlkpsir.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tpmvawlo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fbsrwgnp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bxwklvaz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gecrkjyi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ssrkkvtl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ulhunakm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pritqnna.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3czsjxpfo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3szzvrfon.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gavnbmsx.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fxkrwjgi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iffpyaes.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3etixxirn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ugrqnwlx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ridlkusk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3brncsbbv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3aunthcvm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3lpavjrgf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qwjsvldt.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kwvjjwsa.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qrfvljlv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wmoiropk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zvjcfadh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rizmwfki.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ezohlckj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skhzevpn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lfezdxfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tinjqyks.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wpabtfyn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bkzzizsw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3odbxdscx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqwgucra.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdctaezq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pvpzgljs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3blonitks.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3yamhbcui.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjbwopbn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3sidxrvaw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dumoqhgb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mletfvyc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdcsietx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qygeikqk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ldleoibo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhhhmsrg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gxqprwtv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3xpsqlujs.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjntnwqt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3eqnwdjvs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgknzqrt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbbuhndx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhbvndbw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qbihrovm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qojmranu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihrfylvo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3fcxocfmi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ldwsirbq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3oazuqcpv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qqxlwnle.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jwcojypk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qahczknh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3amnxzsho.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dklibmwq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3camutajc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rkcwqgze.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3jfnuhcmc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aqjccuxm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qcrtmdco.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jwqcnneo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fzeebckp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3gqdbirtw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3plkvgoev.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yfrdtank.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vychftjg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ocyopwri.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vsrxovga.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wdmwmday.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zflamwwu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rjvsutdv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3cqlmafdd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mqncpaoz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3psypfoen.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ilmkmzuf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3itgdfvvx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3djkakcyn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gqshwkhx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3goirlsjj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3temzhiok.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mpinyuqm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jkpropuf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqeaidi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ddzatbcj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jiqbegzz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3pjxomcmh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bljbrpzf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wsrfgnoz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vublbnqx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3pklvccwb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3modhpiii.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3inwvsikj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnzsnkbw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3yevjemhr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bszgrctz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bukmokyi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zhjfyyfi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dfprumbs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjnyolmv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3unjesuzf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsejtnlg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dsacvnga.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xszajtyv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ghpuposv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qumhxgbe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3bmjudejm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zzfeqvwu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3swgzgqnw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kfybklni.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vtbeodih.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nxknjifs.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3tsnkabsr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jegujtuq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wdbzuhcv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qdxkculr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3loeaalbo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nucirabj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ijurgrld.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3tsmjjvkq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ecambpam.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bcpizsyn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3gilpjpfj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mxxozliq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3amdjsczw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tsnnrwqw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3swwiwipo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3omglcoat.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3elvunbvp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xxxykfta.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bwehorsd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3agtrciyl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjcjgrcm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3fcvdupww.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xbmhbcnc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uykdafhs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nlroxahy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vjxhbolv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3clbjhkkc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbufxrym.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rgnxlnpp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bpzvsqsy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dkbarkaj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3twlnplty.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdkefytz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jtdulpau.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ttvaupdm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ruoaynlc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3tiftshbo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3qxuyqjfq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ynsxaswu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlxilxaw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnqmwnzj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fqubmqfc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3menmtokn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3arwqkyqb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kdgfjgkf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bvwqchre.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tjvmadph.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fgdaacqe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3upoahivc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wayfylpn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrgrfxxu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qhdyghby.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3aarjwkuj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3skkzhqqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odjtofvi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3eztcnwex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgwliwxg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vbanhhhy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mqyjbbqz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lrgpnram.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qvsbcbhg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3iyumjkbr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3gwxibwrn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xebugksz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3msaywdpr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3leebpeto.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3hksisyxm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3haeiqyrl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fkqezgfv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vwggcgzi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rzsnyplb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ghwqrwpm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ailckfbl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3dgpvgndu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pmssgrom.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ojprcwwj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qildrahz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bgyeeacg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ylqraodc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kydyctpb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3axdgknxt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gaksybkr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dslvrzcx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3botonejj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ohgeqook.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ncipsjjb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rzibvlxm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ocqumqyf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mnqihawn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cquvnfug.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ekgnaqgq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vzgreyls.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dfxkrpbs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jrglhhyl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3axolbrkj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zxvmltvh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vuvuuxpa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ygsnhtxt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3dxofhqxq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3npgaeezn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aosqltdr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vfivtywa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xfyqeqyz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hkjvzjlh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lrppnyjq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vqqlbabs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tbhwyoxh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ifxfysbx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3apgaqnhr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ljvixnki.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3blteukbr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3kztggpky.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3qszpzlzb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vdrqaofn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3urcwckwk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mshkiktq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vhovjrlv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3taecuzza.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3crzfgofe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oxtbaikq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mjxjdxux.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bhoqgcrk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bguqobui.html


<!-- 参考信息 -->