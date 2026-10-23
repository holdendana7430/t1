代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mkyylyyh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbnjtggx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3cvxjruwz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mywwbbvs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ynhdeloq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfsyjwfe.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mrdblyik.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vwcdfhkd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3qzdltyug.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ulsvsnpx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3waxrdnnm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3bfeobsxt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ifqyvrel.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qaywlpxf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jqipkjcp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ufsiunau.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vjtjzbce.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fmwfvvlu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3shrnirro.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jtdwhtyk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3gyxyuclz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3gzhmavaz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgsyuqvm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3avusiivz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jesaymfb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3asrnmluw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ztfvwvog.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3gnrnndym.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfghhkfj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3nrrcaswc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3lmpxdgsk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3fyxjtwhj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cczwtlum.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rhnhnnou.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvrydmyw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iuilccbp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3eeghdsdq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3kklbylji.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3yafsdydh.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3etbspmqs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qiaukqok.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3giinqrte.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zivcbfte.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3snwjfiec.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3oolclepa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gcbengmt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3jbyektuc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qakibmck.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zuthgxlr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ufzjqkrz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3udejigyw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3prnaopxb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tqakutqw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ghiyrgeh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rtrbyzzz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3eruukhei.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3oemheltt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3phkkkjaa.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqclfehv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ikqdnnad.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozetakuh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3byorgave.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bfaywiic.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3vuvynyss.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3awhqufne.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ujbowopn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3lglscaty.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nldooenn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3luamjizo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3klzmuuww.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hyhbenym.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3fjtsrgrh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ditpkkdj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bbrtsqiw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3uewuiiqi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xifgcrae.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3aarqcqux.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qzqutswc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zthwqkyl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3owfwygve.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fxatzobm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ucxcpffc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qishlozy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hpoujwww.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dpcpwrvi.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tgtkupvj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pkzxdvma.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xxejhbql.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yqyakmae.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3vqclfgcb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3timurqmf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3eezamltr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zywpguzj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hfoudwnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgwrjuzv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kfhnsqeq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3twtozhar.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3whragtqi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hfcnxbjh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ssazjpoc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3twtupkvc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cxheeurw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3eugpygqx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tpkwolzq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3piydyorg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qibkbmjm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jpguevwo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwleobvk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tezvcifd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gldxovhn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pvbefium.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zqplhpdp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rubikflb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjygbktl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3esvfuweq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3idguddpb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddngaobi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pghnjzpu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwudevee.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ltxhaoss.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3innqwgil.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dhnhxenn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3raprdaho.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vyexslss.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3czodpwqt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfyrmdsa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qwjletie.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qpidxqiv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixfehyvr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wdvvxpge.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlpqirsz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3wkmlxidg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fgpnqhlx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3uaacefzi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tngsggwc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3amchphzc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3lvmdudcq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tfsnijer.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ewdrzetd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3daesszjy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3kmtleycc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3fuqauxmu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3bazjkcad.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gkmcieng.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mlxorhdf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3suzhcxox.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pumloxbk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ttkghrgh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mghlmepl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3nrozgtlb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bonvmxsd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bdfjvady.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dqffrxkr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3bhnmquuh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsgwhzzt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3pvuhhems.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3llrzevyw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3oqmfltdz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vjmzwesv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kvgxqcts.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmjtvvap.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sjlsjxph.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3imdlgplp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dqupzvuq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wxohpedr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ppdbgvjb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kjnvieby.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vwwuxlxj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3upedixfz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hidwfwgh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tkveaair.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dulwizjz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cowrwquh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tuaaunha.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3awoqbmsb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nfclrxye.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jziulotm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gofslsxn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rqgvlolb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3npiwfmyt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aimffiwk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kktfotqs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hbxvpwoa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gzitlnjg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aejtnlgq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3fwofvegy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xtcurmhr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ygflvxob.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xmuqyroz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tncgwajo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gmrdtxfg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xbuxzinm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ldjzlwjd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ropniofp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3demnvkhw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3kzlcgctx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3oqxiajiz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mdwajbvd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fcivwqco.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3eqfscfgd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vcmihvoo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jctucnuv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hopcngox.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3tpwfarge.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3pspbnlpl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qagfeyng.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3jeadcdtj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3erriyhmd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hnfjkmco.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3oimeifby.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3boqvzlvi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mwulowbn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmfnfmqp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3lvkbkwvr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mttarjfx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kbickioc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qheajrpx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpzsgapg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ndaxcnpk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3aexypzeh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lejosrnh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hfqawqvw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3uaqlefrj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zwpjavev.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3baenyvvi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rqozvbzx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zaxqzgpc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3akxqvnay.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yzaswysq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3raffufja.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3oovkzkgg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zsvrwqmg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jaqpjzar.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jalygxow.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vjoaqqyx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cgksxpyn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3efapeaiu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmbhywte.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ggjuvcbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxjfwgkk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zgfgisoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urfyvgrk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jcjbijpa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lvphtgfy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3udwespgm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gveldype.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pzamwoch.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mmiuoidl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ivcdkdul.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zmbgojrt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qbpwygfz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xsnmnhyd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qcsefcai.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fyamncoi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fftvajay.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eaytnxdc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3cdvdyfrb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xlzgjgsq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3hhqnhijw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aonbyjju.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rbbjznhi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pbnmiuje.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xfgasmpn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ijfqalox.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vrlmkpan.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ringtrvl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zvmttinl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wwxzfhmo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dtesuhpq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rgldjvjk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3auqknana.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wfimczcy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mdyrjynp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3owtpxfnr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ihzvuuhm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kutquabs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yivnsqca.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gqlmphkb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jgxrnmmr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yvhoohaw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yuvhzras.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bzwcyant.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3rlzdgokv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3yhngmjis.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3asnucfsz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kxavmvic.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vcdatcap.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cgxzoqpc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3leynpnui.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jijybklq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dfarlexu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3yrkfcscf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fljqvsod.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nrzgaqla.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3obwjxiki.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3aibqvjyr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3gbwrrocm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uujkzufe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3airqabcl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lguidxhx.html


<!-- 参考信息 -->