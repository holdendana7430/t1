代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3juwyuloq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xutmbjos.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhdkbfmd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3euwhrfws.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3xarzykeo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3unqmkljj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkifpdtf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3uqoowkqj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3orgskpos.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yknhqzzr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ahkgnved.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3afnnejdb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kwuxctkj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ocdxosse.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3opwiqled.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mxlovqmz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3xgakrixc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xczqcmvm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qymlbwtd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ocoqhonv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcouldcq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fgynqmlr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vkdkvpqy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qodsebvn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3idbjreic.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3owkucitl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ckaobkxd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lewldalb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xyqectuk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ykrzqjtp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjmueakl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rurvvjou.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bykgqfvs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3surqpxal.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3iipnhtst.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rbryeptd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jlsbilrt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3aaugircj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oreazlkk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3aishpyoh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vewznmjj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3nkajdyzd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ncidljeh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lvnkivfg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3dqlkerqs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bqicnvqq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ltjbpuxv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3doxidcmb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lzvfftjc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3uuemijdt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3izybfwkf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3xulbqpqo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3rcuhlwwv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3amtxwjqp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3lvqlrasq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3icvvzhcg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptztzpgv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qvabqqjd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dqtbwsqg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3pfswznxp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mjdudmkp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3oosxwrgk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3eacnwcxu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ykljdhtr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ihijrpls.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cvxgkecm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxahaakb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjuaxcmm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mahupehr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zrhuahcm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3xaeyzzqy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wbhrbscs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ozemjynr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tgtunsqr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rftskhgo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3obvcacqe.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rzbntfri.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jiatpuny.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lkobwjfi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3bldfmbkf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3glsvcrbh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3eaoyungp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ynorwkyy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3brbxomvh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3unovptsq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lcfsznpa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3vncapnpw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3avrauxti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypdfnqxv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ujervibw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfmtpyyk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zdccyfet.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vhzohcta.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kvnfmcxz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zemeoeoa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gxdvazis.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fdruixfn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vumjrict.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jjthtytw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxgifdsx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cwdnyxlg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kiatwjjk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwyevenm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aqcsckjk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aepqxqoi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3otdbzecc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3cgwsaxfk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3grfdymna.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kawlicfk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ahqhrlwp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3zqhjthau.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvtsjxsa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rpupxnvq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xnzccndp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eafkxrfx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3elbhlvwh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3zgcumelt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ocownvjz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ruqlopfv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3kacwater.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nnldmmxt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dzpikziv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hdiudsch.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lxsvvgwb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3lkgntdcb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3axlmtalh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zhfijpmh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3clifjadw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ywionxmo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lkboauru.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kxlanled.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gzodxauv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3sniozqxc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zfauceyh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3btjoixgp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3spdfaean.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bsgelhzz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3mjxegmtk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yaoepxpu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kkfymbwl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eazbkoze.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tbykjnqi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3amccyewl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3swwxfdvg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3txjeocsp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rgucabcd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3kuuyhfoe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3navibmlo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3amepkhyc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3dnxikgrf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xuekzxmc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3eumzulmg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3iktdlqus.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jixtgjcd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bytxwmqh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lwnqprjy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gyqcqmyo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ybfnhfww.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rhypjmsd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ggkcnvus.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sgqpwsvs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zabmyeaq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vocwmtjd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nuuojfmt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgammfh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppwlbzoi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oqgikhib.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uumjyjju.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pjweeydy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nucxstdi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrpxhyyw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ilwspeju.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vjejvwvr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3juieflwc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3epkrdzjg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wnsxzgkj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3owvuctqu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bsrzoymb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fzbbqnyg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vogxauok.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vjrlffej.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fcjvkrue.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3lcdponry.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pktphmxk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nepibtjq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3anglblqo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ayqiejqy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3fkuuwiiw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3olofcvth.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3mwqvkfyq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bhfeyscq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ilitlpar.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lcrwnrzv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qhdeagtg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3csrlgpoe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wtvzxuzp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3fcubyygw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wbszxzok.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zyzkxseb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hoizgcxq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ffiyezgz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qlpxuoxk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jzzmapvo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yoxmfpjh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoakybiy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3iuxzupno.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xmtstptu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fcvaveya.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijdgrppr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3eagyuauu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3drryggty.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zbbmdcdr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3njpnkhbx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aahcpdnl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zdsmicur.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3otaipgkn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3iioqcsvs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3pwoplhxi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bqvnxkki.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gsdmbjou.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wprpbfog.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3mrwfxwhv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ovccfdiy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3burckvls.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3aziwkmsu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pkzprrij.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3dvgrkppv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ffijjvfm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wayutlyo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3tkrwcyse.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rbrykuwq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upmubvej.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pvqutvih.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hbzpqyfe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xprjgpiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqcjhqvc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fogetmdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgpwtvik.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dbwuehlz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lehtacpe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3iqsuaaqh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3njmingen.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tuodykzp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xswutwar.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rrfgtlcp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yuweczlv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xzmsuuzh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3fizgqcpt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3xighcyvh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3owtvqcgm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3syawoova.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sjgyrkkh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ujdtkxuu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hpilvluo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pirgoozg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pagvrktw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zysmxqjq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hhcfxcjx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3uqqbsant.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hujywuvj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fjrdywao.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yqcynwjx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kniboxcy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3aocneems.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fnybtvna.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bmoynmpm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxyjcjil.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jzamcacp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jsgtqfjb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xqwghzlt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tixtpnke.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3eaxxvcii.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qhutazkr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3dsjwsjob.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jjhvwgoc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3upmyajww.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vvyqoxrn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3talymquz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vpuprrpd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3nnyhvbaj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xgrpvegw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wwrtseia.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fngzqakl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3nyrtgezu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nkxnpyur.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ypbaiyfw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ljtqfgwi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uduazweo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lhpfmdly.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xkuauxtk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bufcrbef.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3jyhcwwqa.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3cxdpqnrx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mygisvwx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kzeikfjd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ngarrrcu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wasvjcxo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hvyftahl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rpvrczrx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gfeikpgz.html


<!-- 参考信息 -->