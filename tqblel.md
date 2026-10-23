代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3rypyyovu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3bisiwcug.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qvnrcjys.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ptwlwfnz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3bdmvtych.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zwuphmxf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kgranuiw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kulwpfwp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nuzvnumu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yootkede.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cioqnmer.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cikhubpu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vjolfnkm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3mqiwnlln.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcbmbwxo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdrgnpae.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcefkrwx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hejjutgn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3czjwwjoq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ppbhdtid.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fqjhpnsq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3bdokvlsy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3xyknbpda.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sotsuona.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wngoyubl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qyyxqspo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3yplswdrn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3nyvdgyvn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3uzxwsogr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bptdriix.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3tzutdebd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ldnpgqlx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gspkljpl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3povqaiwl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lkbuqpmk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bwswauzu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3zjhmoyep.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tdjhvrmi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3dmizjxvl.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3gdrqvwlr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lcpqpagj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3sxctjeic.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jgifaikc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hqzddrml.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gvlfreqm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kdnrtrkt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wbnwwivx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3toldvppm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qkfwpcps.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3zzflkypq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3lslencpe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugtsohdj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fjvvsrnd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bpejjfey.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bzuoypwk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3neoieype.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3waxghgam.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3kzoykhht.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3onfhtqqm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3idsiocgz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3knhhoewo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gpcjdbap.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rlhlvvtz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wwanetlx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdhewluj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dlhxwkfb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3hdwbbiwm.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3asqxiedx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3pbfodzrh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mohktqia.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gozozycd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yopuovfn.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3agkfgqcn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zcwuowdv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ifhwnzya.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3civaaipk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3lslgiqyo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3sczhfvls.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tfklqfek.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3elwimqdg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zsfpzsfq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3szpkbfoo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mnwqcjuu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fzlabtal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwfariut.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3updhaqup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcxemxpb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvydqxhl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rwkahgzr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rcjaayro.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3flhcuvia.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vushwjxg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mzvtczry.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tnzjgniz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zpuxpubf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iltqlkdb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3gsykindw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kkteybdw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukywqodx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3urfgngxj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sumsqgfa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3aeucuabu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3oqnhneva.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3sehcrwmw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hpcdcxwm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3lnetwggh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3eogreanr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cfbeitnd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kifdxgmy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rbhtusek.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtxlqhwi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ojnqsmxh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3uswtdfvs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3mowswgkk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3lfhqxrug.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pfhapgrk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zzusrgwl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vudbrjpu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tdklocqp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3taqyxeqc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yyhskxye.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wcsyekez.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3clxdyapy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3shkbckpx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lzvshjjk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3useoftsb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ihnsvaxl.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hgfisvlv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vimkhgcx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3btvvmcre.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ikjxjwpz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ccdeaavu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xpumowpk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bqmdronh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qfcrlfba.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sgqkzrxr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kofpirmq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xquvewha.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fpgyqypz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3omwhxqdv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nkrvxygj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3yokeyzsi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cqkbaqfw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3waymfnmv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hxcqeefg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ufpykqlq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xuunhdww.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3hxefzctw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3clxasdve.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rzmqhmun.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3jmztjwyi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wyiayhqf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3yxwhflut.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3icupwvkx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3adswlwbf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ydumqdup.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3uiaaikgi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ebuurdmd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjtpqvpd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ipxtfxov.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gtgnrjyv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyfqwkdl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jrkrevxc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mlztfwtv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qpjjhozf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xxgubjbc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3laqkrdtg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3admvmkqd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3luijjzoh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3prluziwg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3sakdhoww.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3egqesgmc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kzsqrukz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zleletqf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3enbyojrw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zxtsdwxx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qtbcbsdl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3olihcqnf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mywuqvty.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3sycfozev.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xermptyv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vrxdtoiu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3oghshygd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3tqvxaqbd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3yozemfkj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zenkpvkd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zenoblzq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bunqkwak.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wvpbgqpq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qhmawnov.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xduukpcf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3phnlluzi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ajfxrtoq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jecutjjy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mruttpsx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xzylxfbj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cdzlaguw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3evcynlmi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tvoypuyv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndheypqd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytsvduuy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3bmapubiq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3tvlrrgrr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3qxyokphy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3nzonsicv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vcakfbba.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lheqcxbi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bvifbuqm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpruzmda.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3drkagvhh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cddlbeqm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3msawfcfw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3amuecswm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3bhinjbhy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3eompjaxz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rlnllvpw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcaoxfwb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfezdacb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3spubbquu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bruhwbiw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3akglklsg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3dlzztlwa.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vvcbfhhz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ufblcfcy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3swelwqqb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zubovcco.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3spkaztij.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3zrzzpdch.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3bkytgeec.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ddzmlshv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eaviaqye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekehomyw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uadfpmos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqdatloa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yazjorxp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hmcnuaim.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mhrwmpru.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kouokbhw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ydflloms.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lzyihxny.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vmdltdyc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ophjcltl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3xtojqikt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kesnzqyi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wjfleiqk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lcklsfji.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nnvzqwci.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kkrawxnt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wskdzrwq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3oamcbegu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lolybyrm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jxqbiifj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3levsvxiu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uogdomcg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3oupjwmhs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3sjvvmhrh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uzaiczgm.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kpyvikxl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mvltirya.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kvlkhtjs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dfxmrvls.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mqlncqkz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3blxjpmbb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bsexplox.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3qrcwhjce.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mworzzlw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kfylwtxo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3vwflbdkp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uynjztvy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dwwoodsw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ndnhhjhn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bxbrxqyf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rwccvhie.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kohkoisx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mutzjqcd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lkifuxcs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ccxbsacl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3begsnjfl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qcwnzeey.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jlayvnpg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pjaezhxj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dnvmbrjp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oqxxncmm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3iqnookov.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ghhjpjfr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifeudzdm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jspniqod.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vsycbzcg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3jxzfwplh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ygxdeaxm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3irdxeyji.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mbggarbd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dkpptlbb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dozwmckc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xvbqimmj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cgycaddy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wvwabhbq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rkaxdqbd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nbmvjxsu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zxavioji.html


<!-- 参考信息 -->