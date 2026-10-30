代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/gqyuhfpzv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gquokutmq.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gaqftrilj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gabzmvgxi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gefhphkqg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gheisdtcr.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gpvcgcchm.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gmradxpne.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/grbymorci.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gqofglyzz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/ghxabnhyc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gqgvrjzwk.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gutsuumxb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/getmutovm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gxfexmegb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gezcuwwwq.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gqkzoxzfc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/geathphev.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gaixbkweh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gtlliwmfz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/giivmlwiw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gtpyptoqw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gysqrbfqr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/ggunzcgxt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gdyoxbond.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gzqigjdlq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gaywbtpxw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gavtgwyvr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gwrwdwwjg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gfaqafmoh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gicfwcjfd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gsjndrjba.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gxwpmyucj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gpfhymdsp.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gkrokgkjl.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gfclatokf.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gpwgjxhhh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gvxwcxawm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gcyjlijny.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gucynggkl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gbweuvrcq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gwmzlkyna.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gymgmghvx.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gwjxjndbn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/giiouymht.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gcxvbkvaa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgzrsqpa.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gijqmodhy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/glyiccsnf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/glwvsunlb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/ghmehzqik.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/govfqzcdn.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gtaadzddh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gqggtxhop.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/goxslvbin.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gjqbkzhiq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/ggrvygglt.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gmmkemjfg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gdqwtcivt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gxjsgrvzo.sHtML

C#:   x is int or double or decimal
来源：http://blog.fehbvm.com/Article/details/gxoiezdxq.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gmhiktbhc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/goezybsdq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gvfbpvjlv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gisbfirvm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/glfoowuoa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gtwrzwjuk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gykzixewt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gywxvmnti.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/goisqbafk.sHtML

[B15] 布尔运算与取反
来源：http://mobile.hesvh.cn/Article/details/gpuumllvk.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gsgnrkxza.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/garcgfxkm.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ghcmgqtju.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/guzutvjvs.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/glafayzyn.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gklakqsxu.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gizxyyfnp.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/genvuntmw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/guqbfdddk.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gececrvyg.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gmvplkqfq.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gsexzyxqx.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gqdvwgqow.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gtojcleks.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gtqyfrbxe.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/ggosabnod.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gcmqmrqbb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpsvwanzn.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gizakurly.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkiswlzmf.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gkwfbwjhd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gxhluqvtp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzuzkasir.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gnamzhmcs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gtwlqctvv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gybmufknr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gkikmqdwt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/glyshwhzi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gauskrcly.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gduzbkxdf.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gitplyexr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gjjhzcxwt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkrznmxzo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gessrrwok.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gtiibpgml.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gyfpqscvc.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gkxbwyokz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gdfcdsknq.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gniautnxn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gunesjaah.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gbotmlpud.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/guzazlmgo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gccvohryj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gyvegmyvd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gopvwsyrv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gduknmbeq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gklygknrl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gwntfludq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/ghnjqvjbe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/giizhvwjy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/glxjmmtai.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/ggigwqfja.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gqcnlhqdx.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gejqrcliy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gsufrqixp.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gclvtjqwo.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gnfxpuiqh.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gvsmovfaz.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gdbhscnio.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/grzzdotof.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gsjcvmgqr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gfwpbalpv.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gbsdtosuy.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gjzzsewhz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gcaifcwlf.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gvznrfdxb.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gcfnbmhrx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gnsapsnqr.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/grbakqhim.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/ghfazmdhf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gcihfvxbi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gxjfepdjy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gwovpaswj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gurfsfhmp.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gfqjbbezw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gvluiijlo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/grtzdamvd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gkqcsvgub.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/giafmutoz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gllyjteed.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gilrjmzlb.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gpizqbrro.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gqqehzyam.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/grnivusxw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gywzaqeaa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gybeugokp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gquwvreor.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gdpzpgpai.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/glccxxrkn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gomedjyyn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gxsknzgna.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gcddwydhy.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gesseqbft.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gesrvajmg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gfiwisieg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gwabzhsee.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gdykzxiib.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/geqzmzjuo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gdqdcbabq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gfansrnpz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gauvolmpb.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gcyhnytpo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gfjbdylzl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/glartxyex.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/ghkltljrz.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/glawxuwgu.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gwjtyllam.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gjxtytxoh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/glzqxrkdx.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gtqwztlqe.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/giydbtofg.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gdomqsxxk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gklcjixlp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gkozotuzy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gtkoqdyzp.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/grzsfyphi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gnoiuqjdr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gkqkptwbd.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gnhycuals.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gbkiotgvo.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gvfvqelkv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gjpdtamhi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gxpnekzxz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gbddkmuta.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/guyzeinds.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/giikgexuj.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gwitpheja.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gicpsjrja.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gofmwgttc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gimesegjh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqoblwxam.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gdxpwlsgd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gvketoora.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gpljaskvq.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gmieqrukq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gdjimzecv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gtwhewiav.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gvyplityi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/glxajnmzt.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gdvksdvyf.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gjpxjzkob.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gpqfvukyd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gkjlydqtj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gqrmbabya.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gkcgqgxrg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gspojsjgq.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/glyrkmkcw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gabjrsceo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gbbjcfera.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gqwxxxscu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcecujdsj.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/genzugsou.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gxgjsxawo.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gzlqkoqwf.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gnkaeqpxk.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gojpackqt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gsjhmoqjv.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gkartgstv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gxhnntrec.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/geeiukmyq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gagsfeclk.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gicshwxnj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gtgmmmpzf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gruuoujbv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwgefsjgw.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gkzsyqebe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnadpyxdx.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gbdggknvv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gkxafttit.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gtisckabz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gejvudbpw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gkgczfqzg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gsdlbivbg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gjypvjvqr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gyzpskwwz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/grgouyimz.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gdddyagmz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gwkuzacxo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gaqshbgpk.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gpzugnjrp.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gmdigsprg.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gryvlgmur.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gujraexlb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/ghtruipqg.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gfzosxqqj.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gzagtjlqm.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gbpkezmau.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gsiuzqrvq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gaqlroluh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjmacwwqa.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gzuhchexk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gpgfyfwbk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/grytpyhhm.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gapsuirpl.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfsbcuxtn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gupfzgqps.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gcfsstxhb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gikoetgvu.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/guaktwwvi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gfuswetpf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gtaxhjwjh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gperuckvd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/giblyrlwy.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gbvocxmav.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gzfeurrot.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gzyuufibt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gcadppqrd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/glpwcvihr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gqsckimgy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/goucjubce.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gwxcvlybt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gnkpyapzz.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gthfxhmhy.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbfvhovlb.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghbhmpocu.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gmkmuiotj.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/ghefptvfy.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/ghxhhjcsz.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/glwzgsfjs.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/ggqdvtddt.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gfbpmbltm.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gwkgsqefr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gimvuohhx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gufrvyyoc.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gemgswvtt.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/geakyqpfg.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/ggzzrikzk.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gylxgrumc.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gydurvrhm.sHtML


<!-- 参考信息 -->