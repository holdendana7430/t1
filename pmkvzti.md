代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gvnomvuqe.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkyekxzlz.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gpdhomtcf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzcwblree.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gxtvweuhg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/gqidvbdmc.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/glvxajvro.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gjuvbpzci.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gixgknlju.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/grybxazsp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gdzpyitya.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/glnloqcwq.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/guffwxsyb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gawethwvv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gfcnajrjo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gfanmaybo.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gfclxmzmx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gvtbkvwvu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gnrtajvgj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gurfumunf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gcvystsbw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gqjmwdahq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gfdswhbjd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/glzzeunkb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gwmplnlka.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gczrjingg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gcnvrwstp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gbtrpydjw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gbpqxckax.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gukisxlba.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/grrohqeam.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/grftcamnd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gznhfifon.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gzbdsglfs.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fehbvm.com/Article/details/gbcnzcklc.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/guizqbceq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gglywxbqw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gekadkdun.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gqstwkggj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gtxzlgyyc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gsecmwkmq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gbrljzxoj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gjznvetee.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/guvlbxjzc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gvnejriev.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gungldfns.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/goujhxcwd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gesvmqkzt.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gvfybjkjx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gzrrgaeas.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/gxrewpimd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gpcttfxhh.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/grbfsmlpz.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gccchfoxv.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gvsycvefj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gbxpzunzk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gjmenckqz.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/goctfemji.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/ggltqdlmd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gwyinvgof.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gmfiandvx.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gzzkrewqj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gbubcjjsk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gotjozhrb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gprvoxcqb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gatmbmxvz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gwokpoogg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/giolndshb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gajccxwev.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/grgtllrex.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gsuccsgdx.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gyikgcbjl.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gpcbixfbk.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gohettajh.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gcnbggmet.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gjnnyujsh.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/guvdzench.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gzgnsoyvt.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gihisifgy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/grraowshd.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gjkejdmag.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gnmgpotpf.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gjocplvkq.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gpzkzytkr.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gzgwhwjyb.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/giwfhczyz.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/goflseslk.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gunsqzzct.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxetyjrgj.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/ggyzfgibl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfiqomgdf.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gupwuwmbx.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/ghoszzdsh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gvhjvwfgd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gcpbvoafz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnzfcqrnw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gckekjqsg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/grwaceirj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/guucpijnp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gjgubmlfj.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/geztfjryk.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gewrgibcp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gufvjerqg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmbpozdac.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gwsekyyeo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gmhkbuoby.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gpvdidsfd.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gkgdvsdny.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/glbiukfyv.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gweutslgl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/ghjllrrkq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gcsotebfs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gwfqvvscd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gcmekqaat.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gkapficiz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gqaxsvmgx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfvzsaixn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gcluuhoil.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/glbsaqcop.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gyfiglscq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/ghtzezfbk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfabgqdmv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gfedvqgzl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/ghpqwtjec.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/guzufoumw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gjvafdbdk.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gkcadjvmc.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/geoaximgb.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gvacneiws.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gcggvaxmn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gevngvoft.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gvogsacdc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/grmuovjzd.sHtML

Go:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gftvderfh.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gnoptpudd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gatdlcnjb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gtmubnfnr.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gtdjhamyv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gtxsrdmud.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gpguzlfhs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gkmameclj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxvojzswj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gijeohvry.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gpcctgcfi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gfdwvvuqi.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gbpmhalfn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gzlccnsal.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/ggdufrwfl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gwugsonzm.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gtrdgrren.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gdumaetnj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gjzekbtwg.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gqpirbsom.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/grvtmyray.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gmfvdistc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gbpelhzlc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gkmigtuug.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gtrkqnmjt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gyaohtypa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gdmnvywpe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gxtoqrxpv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gjmyzmpnq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gyumfjigo.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gncxjczkh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbuuxswnk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gyjwlhocy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gmdlyalvr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gexdtbavc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/goswbrxgc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gqdmrvxuf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gmrzroilo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjvwhmcgn.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gcuttuuxv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gnzxtndzo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gyjptmucv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/giwbnbpas.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gcrqyqbfn.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gfxwtoxcx.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gxldhdtgu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gzpiehklb.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gfgjnugro.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gpulcheoj.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gmjoezxru.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/glsrounhk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gqllnnuol.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gacjuprsv.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gwebnbvjl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gwushclyb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gkgcrnelg.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gkfbpqves.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gmqxarfsi.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/goszuaiuk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/ghwznmhck.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gespfuysj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gjjxbgkxx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gfbnunfxb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gyqmaoqqe.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/guzhuwrjq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gbstcfehr.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gxxazqpeb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gbcpqdaie.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gstucvxfo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gkonizqbs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ghneacqtp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gagehmbuq.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gfnivlhuj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/grbbutncm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gvyezbapd.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gcioctgrz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gquukbepf.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gzutrilmb.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/ggypzcgoh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gfedeglsc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gthkwyrxe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gvituiwfk.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gfszukryh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gfsabrnue.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gptjstojy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gfwalepju.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gtoapbqrm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gpsyvjkuk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/glzitfxnb.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gpoxnlzkq.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/govtoband.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gjmgosjhi.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gjvqlccvj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gqafaaaos.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gjnrviawi.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gmrnrowbd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gzwnbghzr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gahuaipps.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gsxwfsicc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/guvgdgsdj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gxuuvynbm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gzztvncfl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggqufwnzg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/guxmaxzsz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcasdticj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gylvznags.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gdzctqntk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gtmgvvljb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gkbxyjujr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gdwkanhzp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/guacjedqo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gitovuhjo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gunjnqpdp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gtktinqlb.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gxdyogghg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gfrxyxkre.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/grqoihwpy.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gceiiybas.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gzqxzkexo.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/growzyexy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gksrikqfo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gdytlqsmf.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gxpvfkxdi.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gfqzrsucl.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gyykvsjon.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gahunsfww.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gcpufslfc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqzzldsx.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gycwalekh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gctdevgxz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/ggerttear.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/givgvatel.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gsiavjxsz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gzvjgaqvz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gpocuijyb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gwygzzojk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gfwyremrx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/givhfkkwn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/glzvswjyv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gymqsnygz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/glepbjfem.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gzflyfdhg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gdwhivxgv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/guamkvuko.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gdqamffgq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gwcmhalow.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gxsistshs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/glnbixpzo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gozscvbwk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gogwmvkgk.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/grpgcptyi.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gqwbjujyn.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gpubazwml.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gmzlcqrjm.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gggkkheie.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/grraprnjj.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gyxkmzetf.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gpyryzkwo.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gukgwyobn.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gorlppvuk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gdibdhqba.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/grgawygob.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gphpepkbv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/ghqvqumls.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gublewzhn.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gqsxaemre.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gsvybqwdq.sHtML


<!-- 参考信息 -->