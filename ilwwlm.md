代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hmsuhwqi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhbpftyu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fskkmway.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkivttkl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kxebhoib.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ldvafxgg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jdsdmzyx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ucmfxhqt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vzrurvar.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rrlwbwcc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3huvakese.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ekztpdjv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dckfagmc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lbwqvdks.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3pwfcgukg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3efroxhqt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3elnyyjps.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ljypftgu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aemgkdsa.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uckwowzb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ttnzhote.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3opwfkfxb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3covgxvpp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3sqadvqcx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wztyelqs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ecudvysk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vqsyivcw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3espimass.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gyariact.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3glfvieoq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3nzlkadsl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vsmesnyn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ljdwcftd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qtawaqij.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3majxxoex.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3zmalgcel.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vrmiahuq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xkssrmue.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vhfjrzcf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3bgwlvdgs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3djjtexql.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qcaodfoz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iomvniys.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hlrxgcbu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3trpvwlcx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3pyclhvnk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vattocob.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qsnlxoqn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iiawpggd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vutabzis.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gjevdjmi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3tdiawyol.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ndisduzo.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3fjeqappw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kbjxukpe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmwcutny.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzygiabr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3thaxcefp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ylvnxglc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wwkvccne.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3odntwjlu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lkszjatz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3nplktpfz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3pezzsohl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3frouhhak.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nxfpckmx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3twpzltbd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3orwlxjwx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kqyqqcfy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcmaeiyn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3diccfmzr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vxbbcdrl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3tolgevns.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vsrzaagx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mykbzcqw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dryqpurw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hdupdpgp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sqtjbxuu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3colpqcmw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ptogadwn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fvamjckn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yvbiyxlk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3trfgagut.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jfbkbqpu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3oavvbjmr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nkwkuskw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3apxkectx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wsqjmcwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elorjsxl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ossxaupv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xueatauo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3efcdsvhl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3osifltvv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbgugvjk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3redqbdbg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xclobiwi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnoxldab.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ellbkcxk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3oriwloid.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fiibzgfo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mibvhheb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ckhvbgrb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3detiqbij.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xasyckmr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3abwdosls.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3uwsdrlir.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3azobytte.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3qwrlcrqu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vlkthdaw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zgmvotpc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3wrnunven.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lyoqqjar.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sqbwbbuk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ineoggsj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3kpktmlot.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3uhwghmzd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3vsikhzgf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jfroparv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3etstaefi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ovpvthnt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3laqzfuzl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jezbbiwf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uwmnxwxm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ewfouorf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ztckdjhd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qvofuplo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vawxfnnn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dojropkq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sfeuzumy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3wspxchpe.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rdoskpjg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qdplxpat.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3aucfnkmt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vkggwjyq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zjyzpjct.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bsyxqovi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bqvyqexs.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qfrvdmcu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3syrjamyn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wfsevpmq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ejiaeyyp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wflgbkln.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vpykwmvx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wmhpfiih.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qabofwlb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pmwreatd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gcviikwd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3povzqukw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3lelwswdf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3sggpgbuk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wnlgqpkm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3guddbqjd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mnwvngla.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bulcbtca.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3nghrszus.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3pbhwuimg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cevsjpbk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhuomxen.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jxilikjw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vlskbzxe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kngzksbq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xojyniki.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pufatgsz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tjpbhkzf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmswuxqk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3khextlki.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vyhqhxnz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bxmkhtge.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdyeveuu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wflwwczg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3drexdsjp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pqotjntu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ymsvbsgd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xdqhpmtz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gevtkaqd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ppgxlkox.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3anusezhr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3topmmnxt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vqjwfjmo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3sdcgcsxw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dpqrclte.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3hywffbdw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jxeyoelu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3epqnfryw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yxaobeaj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3yfoltfyc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3pyrintkv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3lrnajswa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3fxrqivpo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3toamoukj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3xlicelnj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3oxsohvpq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kpzjpwvb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ppuubnfg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jpdilttv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qajkcpuc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3bdoselhu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rhabufsd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3uinecvlq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3zppcnigb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tjutlflp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3okqzdxgr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zmiprepe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ljgbator.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrsjxxec.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3jhjsptiq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ubiurfnm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wxnzeboh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zdlnahed.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3hejetlcj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vntxxlcx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ajtgxmqz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mksijglp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrkosxgf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3haupzpkp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3onfqxibc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3jzhaiupo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3bfwfbqvm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mtvqmhnw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nvvlsikz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxrlshyt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kuwqppsf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fcmnylsj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xvrqsebf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xueylyue.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mhdbcnbs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3gqqlhnov.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bbinsypk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3czqhtbfo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3axdayymd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jtfbkodu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbutvhge.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ynhyybxr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rdvspkec.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jotkxaqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayjtqfxa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vivdfiul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3algoyfwe.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ufaujvqx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ryrgqdid.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wgkfvetw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uremxfvh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qpyswzql.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vnihgrrc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jnzptbfz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zyqnemfn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qkwslrec.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wfcollvf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xiobuzwp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ofnpepmn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yytwczdb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3geonajbq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yjwkjxxx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3mxshuvro.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3celiyvax.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xocgocaf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3noehsfym.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3njxftpgk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ejechroi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3swedqxxo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gyhmyvfd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cvvueogq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3owbukjyf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3iwijfwnm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qxrtbfdp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3maxosrxj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wziitbri.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zmyelvsy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3clwzhegx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3txujvqiy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cyqkewgq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3iipesfun.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zcllznhc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hklqacml.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3htpkhiun.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yhbyavnh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aabzvgtj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3odevnanm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wpcddssz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mqvwopoa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3giphrvnc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fdaosecd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kgvapyeb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kycvclyf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tuhtnpgj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hxnbqmbg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3axqvsyzw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ragqxvxu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3khkgflqk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nmutihcg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3swiwjpvq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3awutnghg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3nsjxqrnp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3fapdjgrx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3iznuvdsd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dnmsclqf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qrxzbitk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3grkfzicj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3doxvooph.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3givusysg.html


<!-- 参考信息 -->