代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3fzwgscrr.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3eixehljv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3khshghqe.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3qqyqphad.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3vqemhizr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wbmtjcxd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jigtbfqv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lwjzchrz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tcdljtrz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rlfbojky.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3rknbqjmo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hkeerehx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3cpfrnxzs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bwesuiht.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3konjfldl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgcwizca.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3haxzhrng.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tfvnnchv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jlfqsszv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mbayumyq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hspenxcq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3lmmkexvr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3xoxkelzo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwtbhsef.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ixbtskkf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bexnnvyo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3yzvygbqg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jmcjqdbf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3yxlozwne.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihhtmsox.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gzpzuirx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uxuuvdve.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bqylpzcg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ljzknbyi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tlkmurow.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3pcmjecsw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xpgsqlpf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xarophko.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3twglfgdi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3nssqkfvg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3yqvcmqdp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3dfkefybt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hsrwcmoq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3noxhkccr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zdusskua.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ktpvxmjx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ouhggijt.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kwkpvaqt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yozhrbxd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ilvtbaep.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3euqkmmvi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yxzbmndb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vbquxpqc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lqsdxsuk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xvhpobdr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3opvchcjy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mdyefjtk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xqnixqyw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mswootnp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3erukyxbp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fdgqmnxq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fbmnzron.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulhopoyw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ocbvophe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kegmjrjl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmqlfeg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3szffvqky.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qpmruynl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3cealshgg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3imwpkttl.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3liuufxqf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rpyvgckg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3skyjqvcu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lpllsedx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gajanhct.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jyxzvxis.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kbryircz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zftowlht.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eltrtzvg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3msxjfgcj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mpeazkqa.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fuawhvog.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ixxtsoul.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3otifczrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewypfhrt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eghuakos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqfufqtx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3amcxejrj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3srajcoeg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fzrkrwej.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkxfbbwy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tjzjenpa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pdfpcfhw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gpwtqhev.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ypxmwbug.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wzwlqvfi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3drnnbrkr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rjdhdtfm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3njkjlbpr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgkcghas.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rphwubpo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qyklmohg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kdoliltt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zgsqywpz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lelgwgug.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3dmcoovfl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hgpitegr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3axmnfbhz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lanpssay.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckghffgy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzghqfuz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ozwulhhl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3haliuuui.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3rszkaebk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qmjvracg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3feugrxis.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jsjfxdpb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wamhmfll.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kilkypvm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3cwgcypfa.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3hjhensjm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hqcfeksd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kyiozfsb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3sgutauvv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eiqrgrwl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3rybdeowq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yttkwsaj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vxsqveko.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zkltfqez.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jkgzduhq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nxvdwmue.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3xdgwzwdv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3nqjuccfx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3uuagdsim.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3iiglbeax.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pizzyfmn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hgojamym.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ihwdqidu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fsbtnctf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hjeseniw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3guapgvsg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3txpnmyln.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zbxdghea.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cqolilqb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3eunftlcr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mobtrlpy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kqntxxwg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3eommwchd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3velwwbwa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3sxxkstmr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jtuswwax.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kfbqxobv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhozblnu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hptxmkyu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxzasgat.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3jthvcwfu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gjrzxmla.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pxhwwaup.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tqvjujxz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fpnsquck.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hglkfvdx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tmvzkded.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nppzleih.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ioddhmht.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3josaraqh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3oyqukmhp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxekdwbq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3droaiauo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lalbiwgd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jarkhqxp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3lbwlnrnf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xuzlbofy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rxmlhkmc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3atrhhewb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vnpcialp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3nnsoueft.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qjqdmjvu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zpoflrtt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3agjgxrlo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3jowiagpe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rbhadrnx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ehzhskms.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ikbjpmfs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mueoqdrl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3cdrzxpek.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ynrttnaf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rpoocrdr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kghcejrz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ivxlqwey.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ewviwlpa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zbbblvpb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ytrjykjm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3dsmppvul.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3odnsteug.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rhrhhkdg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3kcxyixyb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3iptybfwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmgatkpt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jkhgswev.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ycxoheym.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mhnskcdv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ozllaqya.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3oyjelwml.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vwegghfs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ezrccsit.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hkuhjmjg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tcaofmlr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nukddfvo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmauvlcs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3cqatybnp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3cfmrmtit.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wznwblye.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ykafsvab.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cogcqshl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kujhwsfv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mxsnikgl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ehqgpbld.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3khqjtihi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vouvdinu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3aiblwtbd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3oysukjbo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bojffdab.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3dclvrlqx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3graktcxn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3uwjtvzes.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3snlbhkzo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xjinkevf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkzhzamq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3byrdaoze.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xgnmejii.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyptunam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3luappfvs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3trrbydlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rudnltke.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3keeeuhcu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ahrdohpm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vxnacmel.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ltxhuoky.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3zornzubc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3urfoxegy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ixizhfoz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ofcpgchz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3onbqujmc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3pkwzkwuq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bmswhskb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lkrdabgw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wykgggdl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qarneekq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3unlcujnq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3peggfwan.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3brcslusa.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oeumsooz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xmzmeumi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oisubgdc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ffaevdld.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mqbywkdl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tvcjvkov.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fkxfmtwm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ajanktvi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3cwzgdnvx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nwrdslzz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lmxcnrel.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fgfcrmlc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ivbdtexh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3svfeoyoi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3edzucngg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3azuxkakq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bvfuiudl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3migbucvx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jihaupxx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3cchqylyd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qfdyeygq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yimggwml.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cxwaxurc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3szscxgpi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3vpoeotop.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qbsjgknn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jshlwkic.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oenkshpk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vkofntod.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uhotksoy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ssqqlhmt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qfnsckyz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vtdokllx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pjekwigc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ipgoupca.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3itaphneb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3doarbeuc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nbdukxak.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3yvxgfggy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nssycslz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vrvtzcdx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ilrsazio.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oivpnzbh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ocfuznve.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3kxmqahmt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kjikdbsi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jsskhjhl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3usqghlyo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bkwrrmuw.html


<!-- 参考信息 -->