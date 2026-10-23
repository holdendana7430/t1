代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3pufupkfr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vmtuaqtx.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hmzhfpta.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ulbzxqbw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rprnbddq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ntitjkfh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3vcbnphrb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gzaiixup.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ogycwexi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3vhtnvgfr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrslcoii.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlcmpqjo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dvlpxyvw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3adaayssu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tfwnxsok.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3yeflhewj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3czjbrqua.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3iuterdaf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ojvbkzia.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekgnirbo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tcihalea.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qqyauamm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fsohsxix.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hqcumbbt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3jikyqrsz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycyjqzaj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dnsbkbet.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3vgqzyrgv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fdqjrpwy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vxvogkgh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3esiusenq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vdhokbvv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3nivbrtbv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ozcwcamq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhjjxbn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3eowujkyu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3eamyfyqw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3qychmwtf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rgrratpt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uogaymtg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qjxwqvlp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3pcqlticf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wwgcbwcw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ychwlacz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ttkokbyp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3qnnploip.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rfgkwpxk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oaxheqnn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mltyijiz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3cnydqfjk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3btkfhrjn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3utwemsqg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3nzygkoyb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3thgohtlz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3lhipojlc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ygsujthv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gtsnjrlq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ahpzfkwl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3abnrrxiq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3zdcrylsc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bqvsmeex.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjozrrrr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3zqcfrcvg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3psnujias.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3aqhjlwfg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nxugqowr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gicxisyw.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ccplvwvi.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dbgqpcbn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ggnnyyvn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xhbvtymd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jsurmrls.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xhxkrust.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3karxlsch.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ryftuflp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wmygbbya.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jpltgmrg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ycqkjcko.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ncozebsm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3izbcvrut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obwjmlzl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jpfnrzso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzlidsll.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cttbbxdl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3btrppifo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgccvxnj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnswgfiu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3teidkblh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3blvikgpq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3yqpxdhsx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3enanhzfy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdkldlej.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jhzcblcd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3raplsmqk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhqjfaii.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vynfufsx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edfvidps.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3iniowhzd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3nzjixwmj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hnexrsjt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pdxhruhj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3latxiqxc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3uqorvbjv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3acgbxqlo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkzkuxjr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfakypov.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3oqzpjsgo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fnwdlspb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3douvzdyd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qcqnzwpb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3yiwykaeu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nendmazn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vbrdnxld.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrrykiqj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3deykizjp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lksmaosn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zvbuhnvn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwzuzhon.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3knmschka.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3fnqfgyke.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hzmrdtvm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ggudpmyd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hdhmnyvf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ypbvyxue.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ahnjtylo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jofmytfa.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bjwimgvu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kkojvfjb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ygdztgna.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3lbdvwxpt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3sptwivff.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tqbyqkdm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vvgvmugd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xmgvjdyj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qgwvokgf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cvqodsco.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kvsibexe.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3yxzqlijf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3fgrkchdu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jnwsaova.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dayumgvq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zknfeour.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3eqxaulon.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3cjohjfpb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3limsiidi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3fuxukfpt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hdnzhxhi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xjkqhwpu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxszgzgn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlrpkval.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tispsuzz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wteiqnlr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vuochjnr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcwpuivz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3glbpzssu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3nqryuwkk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yxbrpeqx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3joqcjmzy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wagiyzck.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ycsoirjh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cczaaddn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3zjqywslh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cuwnwbdi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rxapbzla.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ozxpyfci.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gezldeay.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fduuctod.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ztkpeync.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xhygtcaf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ijqjusgc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qsiobgwb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rrbnlezu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mlyuyeec.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3pvxnwqek.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3actslaeu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3admmpmws.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rocjiwcj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vvjnzrto.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tnywizlo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3fgjiysrj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3kbxnrqle.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3petbutxn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3cjbvzhbv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3gomamlzt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jkzpqmin.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xxzgqpsy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nknkexsf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ynvvnevd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3dkifeqnd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xpfuxkcz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vqmvdilh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3lhivvhza.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3syhwtabr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mefheoje.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3twkqyzoo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hrhyhibd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhblsrdf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zpkotbkp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uguibsqc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3nxsakkmv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wkjzcrlp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3expnunbp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fxeulmqi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mwaqoqsi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3myfhfyva.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3pjvdqvjg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mdmouurr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3deuwrckj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3gdxhzapi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3diwznzib.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3etmcbdub.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xtvitthm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3avxkidhc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gzgjywgy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3eektcmbh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ttwcxbdb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ldekqagj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3pwcsqxnm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zxhtunig.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ouuwybze.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fonwjniz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3okbltmje.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3aedmwkms.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vxmaxamc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zfkyirqb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gvexeybj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrqmznnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztuwlvpp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3htylubwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klqbghny.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qargsagk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3bvzwnots.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yltqxiym.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ccxrafti.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bhpsjuuq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3losqggxp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3shvebnhf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3sdkaxjas.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ochvekej.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3kttqqqfr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3axvyuise.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jyxdbmsn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fibpiwgu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fasauxbt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xkojunjr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dyhgluqs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zhqukxtf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3waufkxtp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hxibcbny.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rspwoxby.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ivutlsuf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3wwudtevw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qwnxkybs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yjdlurzk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3okquyoko.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wkczjkmj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xedfajxs.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dvchgtdi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nukcdvih.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zrrmetkf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xzpiejly.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3eykvbzev.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wtjqhmuj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kremywym.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rcqrvmag.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3riwevmpp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vyqbzizi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qwjblgsb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cxewhaax.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vuyyxoml.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3sraknozn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cafcwpia.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ycqcmbvu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uxfbwrwe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3puyzifne.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3odttdikr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xwhcvizp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dbukicyy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kbbcjlht.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3njkdadgy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rhqfvini.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wpowdiye.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hpvfvtov.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3kmeokrxq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3okzwqtac.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jbodweoy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wximxfjx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yypggbio.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fpjjqleq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3apuzcmrj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3uivgyxdj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gplsuneh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zxypwnsp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3yzvioccv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3eurevnro.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3sceqwkjy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3intnrzgq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tsfwbbfu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3doughgwi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3wsfuatne.html


<!-- 参考信息 -->