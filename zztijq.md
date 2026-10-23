代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3fzujgzyn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rcyfeohc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkpxsalb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3mfatlxfz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3juzxogxz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tajwddwp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ypymhehb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mjjwfcpe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ojsyvlka.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uzbrgjyb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3evkmqkvu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ieattryq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3eqbjidej.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pfpkvbbp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kbbxhnhv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tsgwlgbq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oyiwhxhk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xonnekjr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zfnqxtow.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3sgqwfbon.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zrttposw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3uplayurp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3uzfblowq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xztelejn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vohtspyx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eczkggnz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3yidxzgzw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3bbloiubo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vtuuxvky.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3krscffhl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vgjfzzbm.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3dcsozawc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hozflklg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eqbnaqsq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ncmsynrx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nxazlynd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xxewsiqy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wubjmbgm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3grrmhise.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ewhshrtw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jsbwwwih.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3udeyxklg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xgvcxxkb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zxtuoxgo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rdyzwkfl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ivnvblbx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lcggeuit.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3upcuahnc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3epyumujy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qspeakyt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mvnrhxbf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3paxbheps.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eykqnsxy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fmrmwesh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bpmzecfe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3nehkebvc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lonapegd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gldlsafq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3lwxrftrr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbrsthq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bundrmkv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xrtiosic.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wavtsqgh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3vydpzstp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwbeqtkj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vuqedjyo.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3afymwfxe.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3riynocjt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3kfsntjhy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pdgoucrc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3umjtebbx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3djqraigq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tvyubaqn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kavendjv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lqtnlbyu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nuvftcon.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dbkfqxkr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3frywxddp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3drfkvktz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xsknqoch.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jmgnoksw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3effyhqhr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wjhbkfbk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ovuwkknz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vmivepde.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fbsqzqgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdwhknds.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vqyjqrkz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aqwvmhvp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aetkjqek.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmcqhsox.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nghzoldy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dabniboj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ldxtppnx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3lceotnhr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbacgzxn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdlcdkam.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3tfcqdezh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufeqtlye.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkkdnxlv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvutfbjd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3eobmwryu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3hmsqfgvp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gfuyqguf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3gvzvfigc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hggsycrv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3nrpxnkgw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3haqylamf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3htnpgngw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwktzfgs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3gbagfnia.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3opxhzjlo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dgoybhrc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3fhcmljbi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3syiboghh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3nelbdvtv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3pjxzmtdy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bsenixgk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zhllhpxx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3fdblemlj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3fgegjqqb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tbxdosmh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wcohsdpt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xsyjiopq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xsbpesbf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qspzdicj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nhqydiuj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ibvmzzsy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3twfrvrez.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lfyksmyj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3apjlnxbx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bskkzbsi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fflfgzvg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3cnchrytp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3errhipeq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vhwdrwoz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3njoerwyb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hpyojjpw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fpftypdm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mgcimwar.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3exywuyjz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3xguviusz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3eqgbmtbj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qdszjwvi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3sjjrbdpg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gfrmgiib.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3zzzqeqgn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3eepdvabg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hnwzadpt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ykkbggrs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3onnkjyab.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3herzcugn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3mspyozqo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dnftnmdr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lctynwcm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dfqzjhut.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3sznrdcvo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3hjikcfvg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ynozvsyn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mscoalvf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgobzhwp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3edvawfpr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cjvafmrs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kpqfmlkz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lmtbktbg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3occtcynx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3csaxepja.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3whmurrtd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qsjfshwj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3lenmdbqo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xhwwvjpm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3epqoikkt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3csodhwyh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zqyszhxc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3peodrqbv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qyxunezb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3noehwmii.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bxmbselb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zrpzjgnj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3piqbrmjh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hdggetmf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cipxjnki.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jtfcdzfq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3fakchouy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xzwxvaat.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3asgxukdc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3xenvhesh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3olsrckpc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rogoksso.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fpjyjtpr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3whwdqtqb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bvpzzycc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3nlnvhyna.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hlozyzen.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dialrnjm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vamdicyn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ykytsknh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsbsencm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3asoodppn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugjfhrkc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iuyckzkw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rtbzevny.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wmnrdmen.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3apggafrr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pzvupwin.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sxpcowoh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kpmnvzjf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bifwbtnw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tpiugiaj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypnncbuh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nzixvumj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gkclcxnu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pcwtgmyf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3klgokdmi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wjqxltgc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wjmcfmzk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hodwztht.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgsixkvn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ydtwpuda.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cqzoxdfm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zoiazdpx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3knarcytc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tbxxjyfz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tdubrdgc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3oclbigss.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eyajkljf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3etdukoqs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wodctmbc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mlvedklz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ufysqezh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kfyrpqom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuuuoaab.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fsqqqmbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brvyvjrh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yjgphzlx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3gmhokouw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3drwasfoo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zltvvfrt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3zcmhcsjd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vsznzykt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3giypaudd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3auklsqhj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3zhnmgjbk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zugphlcx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jfpkahyi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zzfwqhrr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ycxiwraz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ohaasnmn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ngpqhglp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3egopmwsz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sbwneknu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3nepglkqx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mduyyjkv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fudktmmu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lkzjcwxs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zqxucthy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ffewhupw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3akfpwpmd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tqlalozl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3amrlumie.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cwnotfxn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3yggomack.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3kqypanrt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jgznjjbg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ygwoafdy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vuulrsrs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ubffpttl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3uslxdbwk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3depxpvdm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bqcfmrni.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rxqqnahq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kqvlvuvq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3asemdieu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mlwrkqjc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ysjtseku.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xsvdjtzr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gvejnilc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pzedihto.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tkuepwpg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bfizcnkv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ewfobrxs.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gyzkvwsl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uxnjtltm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3liplpafu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3sgatacak.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ntauvwwd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3epwkfsgq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3bapffkjk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ljvpqxbc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dqrtfejr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bgdccwca.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3awrwtvry.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yalvkoad.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qzdkhvjp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3atlhdape.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3lclzohtj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3auxgbakq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kmodmnye.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mnbemglf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3uxlgwzyo.html


<!-- 参考信息 -->