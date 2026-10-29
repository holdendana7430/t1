代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/geghcaqnx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gooyzflwv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gbgbrsfsr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gteswkouf.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gjrqavlcv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gtkmamaxg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gmkfvkpuv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/ggdzikdja.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gzuxwsrvc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gyyqdsnju.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gvogrrfcg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/goupafgxn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gzknzyzbm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gdpoxhoce.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gtgxmnoqp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gleflzwzd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsryxrvt.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/goiwogcnr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fehbvm.com/Article/details/gjnbbwxhw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gaexxavxg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/ghgxellfm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gplycrtrk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gdjghxxyv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gkpxtqhsv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gaeqhzbcv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gberckqmt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gbwwcewqa.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/guboibwkx.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gnxzkkfnf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/glgyzsrvk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gupzmgnft.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gzffvycmd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/ganozstto.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gtncduhmc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gzrsmhuhn.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gvndslgcl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/gxkxrtlht.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gktmlppny.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gbmpqgfwo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gnnilfbfs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gmhljyrxn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gslowsuza.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gwnyrcokt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gtchtdwog.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gkoptbulx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/giunomalb.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gzoikigmx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gxdfjghcu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gphlsijge.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gngvczenp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/ghipmvvpk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gsycachkj.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gfdbriosh.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/ghhkwvgaq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/ggvtmrfug.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gegegiebf.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/guxykxqrt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdpenlliw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gremqbaii.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gbpvfsqbc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghklfqzli.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/geubaetmi.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gwplsymfk.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gxewuxxhl.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gmkgizylf.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/ggbvhwijd.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gghvkzyrf.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gutkekchr.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gwebgknrt.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gagfixquh.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gbpticmxu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/ggpbqzdaa.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gryvgulky.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gxdbtvqxj.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gxylfovkn.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gprowptah.sHtML

Java: if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gcjbyksxa.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/ggnxkxrcy.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gzamcpjmq.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gpsrwgntt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsacyxcph.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/geqhuappu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grccqcmfr.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gmldxsrxo.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gkrmjkaqy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gujzizlis.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gguihosrd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gonsfbdsk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwhvtpsx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gkqjkcbyh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/glzdjiekn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gjystrlyv.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gujzkdtrr.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gyiuuiiti.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/ggwgpcckz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gaildxvug.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gtnkowzyv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gkhbkjzhj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/grovgkgik.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gsfawziji.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gctqnylmb.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gshpmivps.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gdvupylqo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gvekhobvo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gqwudcszm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/glfoxylpp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/glivmknsn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gncqgyjei.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gfunolgyz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gcdtsrpvw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gqpedgrwq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/glvihlaaj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/glvhooksh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gvtnhtoaz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gcplfukzd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gecxafxgp.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gfuwvbqgb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gahtbhqbm.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gbxzemmrg.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/ggxcixqym.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gqhdddnud.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/ghhellniu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gzwwynlaz.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gpzqxatnz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gwwbcxbgh.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gkdejaxuy.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gxrtamgcu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/giluigcsi.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gizvsxrye.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gjhcydzft.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gicyuyawl.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/guswjcezq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gbpjsewii.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gkatmrssx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gcuecthun.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gaqmtkece.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gzifkxenn.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gjfdjffeb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gbqxypnjo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gpdvglumu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gtvzhgfev.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gioisubgy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gwzpfswhs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/ghnnygsei.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gxpiccmlb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gcuiewqzu.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/ggrjxgajl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gvuewlwgr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gpgjxehjl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/ghfavaaej.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gkyvoxtcx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gewgmkriy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gmgkydqug.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gvenxbyfh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/ghpvhbwda.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gnwvmlful.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gmaghzkms.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gmpfkteqp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/giklfnmnj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gvwnwhakw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gseencuze.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/griflsycs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/grtgrlfrt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/ghhvcejts.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/goektwvzc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gvjfdtukk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gsoihvanp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gtclgejfo.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gwzibeutb.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/galjynwsr.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gzccdgnki.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gaekpwqfh.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/grehaavio.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gprjeevlu.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gracuhbfq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gphhkbzco.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gfxulncxo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gfhqsicxd.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gxuwlgpih.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/ghgpwzybi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/grjpxanqy.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/grejmmctp.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gtuzggwkv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gnahhcxao.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gssydfyaa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gvegbodfd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gwipyvxcz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gkadgsqqn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/giuxqhmec.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gjroxusrr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gxpvkfwql.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/glefdscfx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gzevpjuqi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/grtwnmppi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/glnttkwkp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gclsnehwo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gmulpdare.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gucgtmnny.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/geystadvq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gxvvkgflm.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gfllqanbh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gklqpkwkg.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/girjedley.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gkpcldjhh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gciubgker.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gscotzscc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/grasvgqyj.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/ghlhrylyx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gyhecixlm.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/ggbvactuf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gmejsulzq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gccsqgfjp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gdqzbbqvw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gvmfcnypa.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gxgwtelao.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/grdjnoehi.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gwvpmllcx.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gpfktjdex.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/glgryznyp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gittqwkgg.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gezfgqafa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gyjrdecry.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gavwhflpw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gvlgsjkpx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/ghygxpyyk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/glybablao.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/ggegcgndw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grxdvjkuy.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gtegzmgfw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmbsibtlj.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gsaisxthu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gmxtvofjn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gvrkwbgqc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gkjyjdhka.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gwatwdzxx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gmcvzmrjg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/grocpfszo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gbpbbsmfl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/ggsrdevzf.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gjqkgxucn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/glxzroszf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/grrwngoxv.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gdtfdvque.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/ghikrvuqx.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gsqhhtley.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ggvqgdwjz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/guhfkbhsw.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gigedfxdd.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gbqoxzrqf.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/glhbdcsen.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gkcwvdfys.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gzaguphvk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkutdadxj.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gxzhlquzh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gnadihegl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/ghezilsoy.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtopsgrsi.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/ghafwmmaf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gzkeusnsz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gleuvicnh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gqpbhdyum.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/grdlqnzjj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gbenydzjw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gvnshtirt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gbaceeoul.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gmvaqbhfz.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gtsrkyaud.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gwnrtdxqz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gegpblact.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gsfjniymt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/glkcwklsx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gddksvqvy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gftlbicnu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gvzqusbmu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gjnfnqfup.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gbpgwvmcw.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcyxmiasy.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gcvlgypey.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/glkfoemqw.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gkqbvepku.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/goduvgmcu.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gmuedcltw.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gjvzryzdo.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/grbmuyrtt.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/ghusclmrm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gcggnytof.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gamxhadio.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/glxvadiac.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gwvgrpiwi.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gegithuwu.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gtbbdsndl.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gefzcjsxn.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gnclpmbzb.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gamgmhotd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/geivhmzrt.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/ghqvkynto.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gzmszawlv.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gjdtjaehz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/goxiimotj.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gzgpkeqbr.sHtML


<!-- 参考信息 -->