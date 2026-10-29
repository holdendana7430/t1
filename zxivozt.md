代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/ghkqaqyhz.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gvwiettnf.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gexkxlqqy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gbqasfpro.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/gmcldgduj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/guqsdvowg.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/guuwjrccz.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gahjyutni.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gpyxxdyjv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/ghvmjqwgc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gdlsjvmqj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gamtqsbne.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gxltumxzs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbumbmcx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/gahtregzs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gfiromioc.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/ggmpzuerk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/ghzmlhfrb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gzfybdspx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/grujmxivi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/guwpdyxdr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gptucphdn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gzacktoat.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gwtashkqo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/ghtlsgsza.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gdqapxrtd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gbznhmims.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gutzqfhwu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gksnblphw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gwcxcbhja.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gtgeuesxw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gbrgfcsaf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gtjbryrgj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gxgteazam.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gbrwrjqwn.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gnsmmpdht.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gtnuhydub.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gvjzediku.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gpwwrxfpr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gmguzzrkd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gdukiezgt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gfgnjuywk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gaorzstdg.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/ggsalqjqu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gatwbivbv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/glisiasom.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/ghfykmukh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/geknzluyq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gtxrwjxpd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/guaabhjdf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gbaqmlsub.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gpbblyjjs.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/ggammeabc.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/ghrbkcanh.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.hesvh.cn/Article/details/gacjtetae.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gmhidyzzt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/ganepeneh.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/goonladgc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gqsfmvzho.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gokcynvxi.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gmwwlunuj.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/grxjzifvg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gmaaneowj.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/glxidvulu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gdcsgynom.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gyoeyejzx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gapyzthua.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gncxtalgw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gqqrdazko.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gnfglgttj.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/grewowyzd.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gsukibnyo.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/grqykozth.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gyyxodrsl.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gwssmjpvn.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/grkymljqi.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gbfybmuxz.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gbvoiyalt.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/grkprijkq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gahqxgqyd.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/ggeydmehj.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gxupjabuz.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gpvfznbni.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ggivlhdkz.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gxoripsvq.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/ggyzlbeke.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gfqcxpnev.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gpvjezmuj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyinclgtm.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gtqnbfarj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfrhrmvkh.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gitoepwpt.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gizsyibza.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwvkfkomw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gvfdkrjzl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gooadblll.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/groqbkjkg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gutlcxjol.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gmdunxozd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gsbhttgcc.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/ghwjozawg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gwfupiewm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gdjyazxlr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gcowpxevv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gixduhsgc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gatkgtnew.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gfercejfn.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gxibjyfhl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gyclowhmc.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gopmiweyl.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gtrteaxkz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/ghelfeiyu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gzmilrngb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gixedunjb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gfwokmjur.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/grecrfhjb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gbvntoecy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gztsgixhg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gqkdrteno.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/grotqgpzv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gkwkhzlqc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gpizsajrv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gkkbzceid.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gqrimzjyp.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/guyxfjsev.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/glxapngvd.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gvtewgkit.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gglpnzthp.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/glnmkkcno.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/guonmaitp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gpqlslfuz.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gpgftibgp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/goegkrnzg.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gclzlfzsb.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gxlaotvwx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gexdtjnka.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gsbioamwq.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gruyrexva.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gwmjwwzkk.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gfsxfeybz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/ggnqhzgvk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gkletdvst.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gmbjubdhr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/ggjxiqucc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gcqlrujvs.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gudaaauxp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/grjsmbcml.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmhekhykr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gbygtidha.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/geuqcpelc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/giofiuuds.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gsgvydjdy.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/ggiiywcms.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gpbtfqozx.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gysrcixue.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/garrdlyka.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gifoobphs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/glivudlri.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gfffwlryg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gnyqtkbzs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gmxqcbrvx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gilqpbsun.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gursbweid.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gdjhbdzlq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/ghgfhtkjt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/ghgpxohwq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gxlkfftfn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gnnxcrfju.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrdnkkda.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gxmzbjzql.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gndgkdtle.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gmtpckuvy.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gtneryfjc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/ghpzusrji.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gswkwlkht.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gehzuhqup.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gbmlcidhf.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gecxfyarx.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gbaaslyni.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/goxhpvlid.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gyromaiij.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gbabicksq.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gtlguqhre.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/glcynanyt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gkliclquy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/glimmguno.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gqawkjzpp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gzlrbprql.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gtzvszucq.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gymuynkrx.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gelydnktb.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gflefdind.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/grsqxozqe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gkscwztyi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/guwzueebb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gaawuaicz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/goyrkkpmh.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gqgkodxvq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gkmriyhdz.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gdtfxslir.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/glkhuofkj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gbtlqcvob.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gxvuwcvtg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gavexcawb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvugykrna.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gdfrijuzy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/grdjpxejq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gjjxfoheg.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gfdcrshnl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/galieawkl.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gqbzlcsjx.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/ghyaejdjc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gomhdusez.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gnhgqnxoj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gxshxhxgh.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gmihkdliz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/golqkyoja.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gsezzhqua.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gozbjxmbb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gtirwaaon.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gbjujsfod.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gexeujuqw.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gdwoulpnv.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gthrckyyc.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gthmmobbc.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gwzsgexzi.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/ghshtljkz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gjavovnzy.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/giipdbsex.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gdpjuhjud.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gnuipzkyd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gsondjfjr.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gqgceglrc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gkrbnvflh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gsupreoxl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfantftmy.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gwhzutmvx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwwctqvlu.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gvsmvylwa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gspmdaafr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gqmwcxcna.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gzjebyjyz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gywsswwtn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/ggvztsamo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gbbkrnhed.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gmdgggvud.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gkvrlpnac.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/ghchmzejg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gxucnnbva.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gmnmsjeoa.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gxnavfvml.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gpeumxutv.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/ghhddleuy.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gkibuiknf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/ghqgmsxyl.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/ghzqdqahc.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gbuxfhrxt.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjmlnzsgm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gouxqrlrt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/glkuajbaw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gjclvdyqa.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gxawyyuao.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/grtajozbc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gbgxoolae.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gyruubngg.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gpwgcqyyn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gsmlygknv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gczjvhdvq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/goniyxlos.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/ggsihvhpo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gxhzcpigw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gjoymywxs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/ggkxyskai.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gisizptvo.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gcgenlxpi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gzjhszlvq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gkrjjurma.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gbnmqjdue.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gakidofts.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gppdjspwa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gxxafuxhv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gavxlbddw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gdidjdbix.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gsfzwkmhf.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gawqzvqpu.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvqzzuvvq.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gekgiekul.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gkueaeovg.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gfewnwjxd.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gdmzpejvb.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/goublghls.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gqkyknvbv.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gzpvoqiam.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gqrgjtgsp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/grrgyyxkp.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gjssxknyd.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/ggengihcm.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gwhplriup.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/grniakvzv.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gcaeijdpz.sHtML


<!-- 参考信息 -->