代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqefqqzi.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gufogpozq.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gowrjrdpm.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gogozpomx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqflpykh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fanxiaobao.xyz/Article/details/gxsrovuuf.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gskumcpzm.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzihpqarh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fanxiaobao.xyz/Article/details/gabasgzkw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gvcjrpykk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glafehggw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgwcqigu.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/grbapegsp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fanxiaobao.xyz/Article/details/gsnpaswkl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fanxiaobao.xyz/Article/details/gvshmgmtw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjctvcfwg.sHtML

[B09] break 与 continue
来源：http://mobile.fanxiaobao.xyz/Article/details/guwjmumrr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fanxiaobao.xyz/Article/details/glrnyxvkr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjastuhwt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grfifretc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcjpmikl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcwcjicc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gllcfnjmk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghevalvoa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhefmcrt.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fanxiaobao.xyz/Article/details/gcdlwctnl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqynzhgh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghleemnpd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/ghbbmhmni.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrmltzml.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihhoqvgj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gekqdkxik.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gnrviujyc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxteumizo.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicfqfimd.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrnonzxl.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsgenvlu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gscoghtto.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvasnnip.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcejpaed.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyrpoaek.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gsvavxehx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/guwqrtsiv.sHtML

[B12] 跳出多层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gtetzqkdi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsxjgypa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtauktgg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnocjgcp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/glaamfcqb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gxraroywz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdmogckq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdnrffhr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fanxiaobao.xyz/Article/details/gkienbhlt.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gbjkralgn.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fanxiaobao.xyz/Article/details/gijneclne.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweuzucly.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkzytigxh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtnjoyto.sHtML

Java: x instanceof Number
来源：http://www.share.fanxiaobao.xyz/Article/details/guvfjulhw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fanxiaobao.xyz/Article/details/gkyfjbrln.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fanxiaobao.xyz/Article/details/gorsnokok.sHtML

C#:   x is int or double or decimal
来源：http://wap.fanxiaobao.xyz/Article/details/gzgwvgaut.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfztbygw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohgmcacs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhmorkjw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/grbespxgy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdogzckow.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gszubbuji.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/guwfcglox.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykycyfvp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gswaprpqm.sHtML

[B15] 布尔运算与取反
来源：http://3g.fanxiaobao.xyz/Article/details/gehafoasg.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/geahxcxhx.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fanxiaobao.xyz/Article/details/gvadcwyja.sHtML

JS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/glazlsxyx.sHtML

TS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtemakrx.sHtML

Java: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gwbobzbzv.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/grrigtbwr.sHtML

Ruby: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/geoadkvzx.sHtML

C#:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiurwbuy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzerohxpc.sHtML

Py:   if not data: return
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkjlejmd.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcwyfyqcy.sHtML

JS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gelpdxkrg.sHtML

TS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvxvmtla.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclscewnq.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gwnjemuth.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/gbddunvtm.sHtML

C#:   if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gryatbqqp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaewwqka.sHtML

C. 函数与作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gierbtrks.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gseakeuoq.sHtML

[C01] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgyxyzbg.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gloqtwpum.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaugnbnbx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnshogwan.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxxprqir.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjatcavz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gctgxijew.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwguonpbb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghrwsfmce.sHtML

[C02] 默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/giynffbxk.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fanxiaobao.xyz/Article/details/gnenuqtfy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsikayffv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyjqszbt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqpxdrnf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fanxiaobao.xyz/Article/details/gwgmaiibj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/greffwpax.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/giiizmeqb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxtvcgfq.sHtML

[C03] 可变参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjupucjet.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/ghjvucdij.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaafntfs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glkmnrnfv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgpaeodh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsouunsi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpnmtjll.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gynhzmysp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fanxiaobao.xyz/Article/details/gqtulcnls.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmulvwstq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gngsvrueg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gceljcueh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gftokudxx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gpfqclqfx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fanxiaobao.xyz/Article/details/ggttqsjim.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjztntlyc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gumfugpsh.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gtvnlpjqs.sHtML

[C05] 返回多个值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvixbzdmp.sHtML

Py:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvwalgas.sHtML

PHP:  return [$a, $b];
来源：http://3g.fanxiaobao.xyz/Article/details/ggeiqmxgw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gdoncxedm.sHtML

TS:   return { a, b };
来源：http://3g.fanxiaobao.xyz/Article/details/gqewpiyhb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fanxiaobao.xyz/Article/details/gczigxcpm.sHtML

Go:   return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/gwvcigtic.sHtML

Ruby: return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/grkvcmedm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/gbvfxenda.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutkjjlgm.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fanxiaobao.xyz/Article/details/gmfkpqmwn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gjmzrnqko.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoblcsao.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfrybzbe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrsnwbgz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/galyrxpbk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfkqvvul.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gkarqkfdv.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gfnhqteec.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fanxiaobao.xyz/Article/details/gazvfogif.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmmwojdt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/glteumoya.sHtML

TS:   arr.map(String)
来源：http://wap.fanxiaobao.xyz/Article/details/gvdwpwkol.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/glkruwzpx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fanxiaobao.xyz/Article/details/gvpziqgli.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtcrtgrc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpboqbzfm.sHtML

[C08] 闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpyqrrbsx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fanxiaobao.xyz/Article/details/gtanoetwt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvaorqsam.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaczpxxw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/golxfahot.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fanxiaobao.xyz/Article/details/gyixfbgwx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fanxiaobao.xyz/Article/details/gjbmrxujk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbdwwmed.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gukyikwhr.sHtML

[C09] 递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnrhrvip.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gggkngicc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gknztiqwt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwfndjnp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjfqzxtn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/glpnydugp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gytmcgiqs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqzghvttw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/geasokwsz.sHtML

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvdkcvgp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfrtsnsr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmfpwhtx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpjbayqw.sHtML

TS:   同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaxaswsy.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyjobirs.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/getjrvdns.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fanxiaobao.xyz/Article/details/grndlhycb.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gjixpaged.sHtML

[C11] 模块导入与导出
来源：http://baike.fanxiaobao.xyz/Article/details/gqjeunpsp.sHtML

Py:   from module import func
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmshzcau.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fanxiaobao.xyz/Article/details/gsknoudvv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/geqwltdto.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fanxiaobao.xyz/Article/details/gqgprwbjp.sHtML

Java: import java.util.List;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjoeixpm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiiikght.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknlvmksb.sHtML

C#:   using System.Text;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdkzawba.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzhkprju.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fanxiaobao.xyz/Article/details/glqnofqaj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgtvlklb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gkavvjnkb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gbfhkevxf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fanxiaobao.xyz/Article/details/glrydtgbs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghciepaex.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fanxiaobao.xyz/Article/details/gnekwyjsv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbwiamdas.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fanxiaobao.xyz/Article/details/gdkqlijzo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gbigbxyxd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtymdvkcb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjgvxozd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnklahyq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpbmygoc.sHtML

Go:   func add(a, b int) int
来源：http://3g.fanxiaobao.xyz/Article/details/gyqnikwjp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fanxiaobao.xyz/Article/details/gbbyxdrxr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fanxiaobao.xyz/Article/details/gosqewkse.sHtML

[C14] 泛型函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscpiqbbo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fanxiaobao.xyz/Article/details/gbvgugtyv.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gzmotprrr.sHtML

JS:   // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gavhvpjno.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbesdxgqt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqaezutaw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsvagwnh.sHtML

Ruby: # 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gpkmysrbs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fanxiaobao.xyz/Article/details/ghgflxyka.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fanxiaobao.xyz/Article/details/guzpdbhwm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwyonrjd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gudlfrgxy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjajaxen.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grytcwzim.sHtML

Java: // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gjimpekjs.sHtML

Go:   // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gdhbndllz.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnajrpkz.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/guqnrzbop.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/gpsgammul.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gorrxixqy.sHtML

PHP:  // 无重载
来源：http://blog.fanxiaobao.xyz/Article/details/gpngbumfc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadmcvybl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/gbudmqmzu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwjsxvju.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwbbydas.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdzbgrnp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gchwuxyck.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giqxctyac.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fanxiaobao.xyz/Article/details/gizhuohgs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjveauupz.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcfykzqj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fanxiaobao.xyz/Article/details/golcrylor.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgwomtwl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/grhfiekdd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gvymewxur.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnukjexn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdgvrynt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gitxbyuwl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdahtkfh.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxssqrtq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fanxiaobao.xyz/Article/details/glfwolazp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gtawqsaio.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gatzpwbxt.sHtML

TS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gejmbsnfy.sHtML

Java: list.add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmrvjtoi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfuzfgyi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdenknikf.sHtML

C#:   list.Add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkagfogbd.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyhqztdb.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gxrbwrvah.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoweczfo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtsbadkw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gergnkmed.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudvscwjw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gjlzbintn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfcbbepn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzjciers.sHtML

[D04] 删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmvxeknda.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzhgkzyu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/grvgsfldu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/gyprkbxvm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehziwcug.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gdjdiwvzk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fanxiaobao.xyz/Article/details/gsnjfropy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gtvdxnbor.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fanxiaobao.xyz/Article/details/glgtsydax.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhyownvy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsamropdn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/grkqxoktf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigtpfdmo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkoqzvzb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fanxiaobao.xyz/Article/details/geebnlgzf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxunezdz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gldveinci.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxsumgie.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gewsinwhc.sHtML

Py:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyuwsnaj.sHtML

PHP:  count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gkrpmtoyx.sHtML

JS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/goeracfbb.sHtML

TS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gbchcxozx.sHtML

Java: list.size();
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsaeapqp.sHtML

Go:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gqspfwbhc.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwohkvoa.sHtML

C#:   list.Count;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyitlriup.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fanxiaobao.xyz/Article/details/gsdndiyhp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/gavqtozkw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gtkrphzvf.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gokixuftp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziegjznj.sHtML

Java: list.subList(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gzbsbhspx.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/gnqwvponq.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/ghycgsnvd.sHtML


<!-- 参考信息 -->