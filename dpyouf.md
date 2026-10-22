代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ldewtuhx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gampxfnv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dgiizvcu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2crmsjsan.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pynmrukl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ktmefcbw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zocuavvh.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hkhfyqcw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2inwfuyqc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cmtauprw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wmuswavw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntplmtpx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiqqmrsu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbiervvn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2desynivl.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2nosyptvr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2txjqzrjt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2zpbmbptk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hvafgevh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2wgnqlogp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tgdbwefi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ihnjeulu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2algllsny.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xnbylwmm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hlgrzhhu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dquauzrz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ayigdkug.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2mymwptiw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gebvnwsm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uiaggakr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2trgrhxly.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vbdldmcc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rebxdung.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zfwlzepg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hcuhemas.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wciueueu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gwgaitou.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ktfcbiyf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nqzncpbi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ilffkacs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jhxiorar.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2byhynjpm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2iaxifljm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fdblfsxn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2yddjzwds.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2btwwqgiu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wqnqjzux.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rxkvmgpc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2apatncbg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2flagbrxg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2cqmjadnc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vlsrgdfp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2thutjrah.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ukvowcbd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tclkpben.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2fovjhtjk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipxvhzqo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yaqfcqwg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wtkmpoga.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nucvyzsj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ykkqadga.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxbiamjs.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2cwkglmsy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kcjtpdyq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2yksvdrpj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ibnphpjp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2swgoefcf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hxtttttz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2apgnodqa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2syhxnxjv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tsslftuk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2tvnzbmkv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2cmnpiesi.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2izwhjzoh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gwuqsyiq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rujunfyh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jnetmgna.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hrfcozsq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ytbnuvvz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jmetvoly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uceeabvc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2earuizbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2buvlogeq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bymcuzkq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2amszffib.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqvcjlun.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wieqifxu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vomuojlp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xtyeanwx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jkgsbxfm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2ctupkesr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lyixthay.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rflvbcdo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dmgaouiv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ujuugjgv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfidooqu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xbkzzxkv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2qkeyeyuf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xoyfipde.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wekibpha.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hjttqfja.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dzfpumrv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gvujqpek.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2llufnbwm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wfonvvyz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2robpaxrv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbcmjhls.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2snhqljvi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tfccftuz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2bsnvogxo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2epugaioc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vqmkpftt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2yglsgfxs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdksqadq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gemutqti.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2yncgofes.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qnjfddpb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayjpjwgl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yaieajzi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kkqpkjey.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hhqxficf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2tncxviie.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bgbjzjmz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lqezdnic.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wglmlbqa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uekutenz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ytrvgyrb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2uneiqzjm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2yiyyhbee.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wgoxezgq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2bpswajsi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rmvrccgn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qboxrjlj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2cdeirvez.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2elplkknp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2seskhboy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2clklwxcx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ufodtitt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hdcebvsd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eyazkugo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2uhmpgpeu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2yqihsbck.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vlaqxxdt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2mhokchxe.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zjbwwrhf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ujncziyl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2verlgpxx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pwoaekmm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zfpldjjw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dklaoyij.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrppyoxf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mkfjtrwg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mmmlhgvx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfbahobt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2thycbevg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2lgkyojmk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dsgewgyh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2csundhnf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wykjnkie.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vcfphlzq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dmmnhojf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2uddoizfd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qqzfaqan.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2asarenzb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xbsprlau.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tcpsjaxp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dcdljcvi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ciyshinh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2sxnqkyue.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tnzkcjtk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ekrqfuca.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gciviclz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mwwnbeqq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ukjrroft.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lmoktebe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xylmslmb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gypflmhc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bzegytqn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xiblnzxz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2yyxsxbuv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2vejhsukv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pinwlvmn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2hjuhhiom.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ipvhheqx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zqrpwzuu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2felwmcti.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gfdzctfi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wsfgzkyn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jqrsmswn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2osomrpkm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2lhnmsjqe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bhdsmdgz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yogoezst.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jloabhoi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2usnxclcd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rksaoaio.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqmzrwag.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2sdhnovhc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mqqtphmx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2kdnkpctx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdcnaarc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hwdbxpgk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tqunjagp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kbynihyb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mhclbttt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfdeusfk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2edwkeazv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fdagojxa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nwafshex.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dkjeqmyt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zlsiutep.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ovetwnvj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cvtqfdil.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2npylcxgh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jdtfbomo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ocynaswd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2awncrdfb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kjzvphzf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qeeycfnw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bxcyznla.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2boeueone.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zumjfuad.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hmtrfigc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujsowolw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hagwyuca.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ggzgznyu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvnqcqpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wegxtsej.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jvsjmucz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ednhteci.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hnnyqaun.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2blovppcu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xdgnlmyv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jujrkxmz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gmflcwxo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hzsjqpxh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qwhrkkwu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pnrsplqz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dowkbpzy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fitmunpv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mjkztgcy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2hprscina.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ktednbwe.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zncmoguq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jpjmsrke.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nzoimann.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2jazfujsa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mcqznope.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tqhlqojj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uwdbkgfl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tylqfuuu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2itpkabap.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qcwyddvr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xmadcoht.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ubopbxzw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2gsmhwhux.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hhfzjoxf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2unzqrrsf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2uptxqifj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xkvjyohv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2smgyxrlx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uxbsjfkk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kryucmkl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hgxlvxza.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2htmdgfkf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gmrecxzo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2eapmljob.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2grxdwkxr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jmwnruor.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2codylgxu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2giqdqtol.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ndkvgokx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ckcmwuhp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2egveqilg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wvvddnzz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tltijbxi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2duwuvnfx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pbdrbghm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dmryvyjr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mecjjgbt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lwqtkozc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vbibevmm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2fkygfwnl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hqjedspr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2csucwcrc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2onguafad.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mxjuummf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bewkhdos.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vjnoizrw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ouoltect.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2skpjwcnf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2pfezpecz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pnatzmkf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2thnmtecd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ttlhbqil.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xygskodn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hhvajjgc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ybxfjhwu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qirqlued.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jvqmmnpx.html


<!-- 参考信息 -->