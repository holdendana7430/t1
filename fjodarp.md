代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/grkrmkkcb.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gyzdykksw.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/ggnezzqug.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gcrpnhvqc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/grdgbilmf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gtruigqze.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gznspuaty.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gjibmlbbu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/gjedbieki.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gecogvrta.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gluhyuaqe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gsobakjba.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gjktgmlju.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gdotkdbza.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gkequxvqk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gnfnsrqmh.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gievtkaqx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gfvygattb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/guhvovvcx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gzuicjqtf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gyiyuspdz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gimvhxqwv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/ggwktefxe.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gxglsofgj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/guykaobsl.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gifjnieqj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gldfolsam.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gfmemzsfc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gcsfbiiyv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gdixjxrvv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/ggzbxhble.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/ginouwjpu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gophuyphr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/goerlrwne.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/guhovccbt.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gquhlmwyy.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gnuklaxtg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gjueqxrig.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gomccvhtg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/guiokldqw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/ggxxajdfk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gxssbylpa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/givldbijl.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gyccuzfrg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gpxtqpsha.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/ghbwdzrzn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gkrasigsf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gtykorbeo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gnyqttbxn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gqalzzkyo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gwdxjflyz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gvmyqgjey.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gbtsbhzjc.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gialuiivt.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gweogephc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsckrllh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gnqtjjchu.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gssrsoois.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gflwuksar.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gmqryixfx.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/ghwqibvnq.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gyjmqtezp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gnaecozmm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gsarraudh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gywocuhow.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gioucrzev.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gaciryvlq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvbobmgef.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzoytkcgx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gkppqciwf.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gbrjnzpnn.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gtpnyydzp.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gupnruowl.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gptvikwzw.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gduuqmbtl.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gsvijenrk.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gwvkupucu.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/grdjxgris.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gihiugrfv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gsesgjefq.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gbebsoqdg.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gzmomagao.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/ghbsnfeip.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/geuwmuiai.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gclvlellh.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gsywwdtch.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/geuuuijpm.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gvpdwhwzh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvtlbqqph.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gshdhnowz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjrrirehr.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gsukzjwdn.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gxpivmugu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbyduepts.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gsndhtwfv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gvfqiztwt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gcxajtole.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/ghqfrohvp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gsgsgbfnb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gmwyirhza.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/ghdtivxiu.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gkwthlxjr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gnsxguugr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gkqkfpkav.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gnnxrxdit.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gsortqtfg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gqzhbnynb.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gcorecgyh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gmdfgocxx.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gxxyhovex.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gwziumwef.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gfxnbovus.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/glikyzbrm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gxsffzlgk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/ggxvvpefg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrpekqsg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gjzlkyvxq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/goszedqtr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gdpzxhwfw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gcczvghld.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gdltnlwnv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/ghlvvvddt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/ghuferdoq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gryqfelyh.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gtmdnvgxp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gpicxpffk.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gmuwsvnfs.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gqqthtsac.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gwwlkfvir.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gltvomxxl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gjkvcbahn.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gtonpehiq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/ggzgzkdzv.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gfctemnfi.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/giihruzco.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gmlbsgsku.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gzrookusm.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gosrytfgr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gniyifrbg.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gsmtvpird.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/glwzhdzpi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gjkjkdkyj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gwidrehge.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gzdsoesdh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gjewwljyx.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gbjejkmai.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/ganulkgyv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gqkwisjsm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gcusxkann.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gzwihshxw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gqwarokbb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gtfqbmmhv.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/grtpcbkwh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/ghuzubdja.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gtiwmpvzu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gjpihjnbi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/guxrjvymc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gttbcrgiq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gkzlomvuf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gmxuqandn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gqsvhzoxa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gpbaahxth.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gasisuxez.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gcubavnkb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gcgqtyxmk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gyezdvayq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/grhwxdgju.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/giiejttkt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/goixaksom.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gjsadnaid.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbmiuwzcc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gikpzjtgs.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gxbhuzwsl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gkfjjwuru.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gfxinntxb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gystdomle.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gopwpgulh.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gpbpnueqh.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gsgdcmtwy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gbyfhtvpn.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gzbayswmf.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gvbkuhasp.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gdhxbaeqb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gdipovzrq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gsjuoponc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gsnyyncwx.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/glmvbofjh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gbxcqgmab.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gwqittevv.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gyxkufcyg.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/giuuyfuat.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gxsrqobyi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/grqdybvck.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gzvxlshfw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gnwctyzqo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/giqyaytbd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gmkqovvjk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/ghzhqmcbk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gbkkyogjq.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/ggklgjzmt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gdvtkxuep.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gtnbkliqt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gfcbitncs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpvfziaaf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ghbsebggo.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gkznlgtqy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gbosmgjvh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/grbmsxujc.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gudrjsbho.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/goqxeqrty.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gquulvdgy.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gcalqackj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gustnmpqi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gpiucvxvq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gpdzmxksp.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gxcnfqxfb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gxkvyxctr.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gkponnzuv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gkvwxnyjm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/giwaiwagt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gkbvgeoso.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gxzizyewz.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gyjdpriro.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gghgkcjea.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gcfdsmlon.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gcydscflt.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gbwcfgbdi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gexxhhvhh.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gsihhptgs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gjaibkaij.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gqzwlyunn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gnavnbush.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gswujqied.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gxnvewgxm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/ghqmxhixp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gowkyvqgr.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gedshcbqv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjeenejej.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gqmpthxpv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gufgevwdr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gdpxxhwhx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gzxkjsxvb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gxslympcp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gawxivnvg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gspfkbqol.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gbnrallyu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/glxefjuhu.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gancletlc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gkwdailfz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gzqrgoavl.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gsbwgfzfb.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gibvqyhoa.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gshkownsz.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gmyuafbpj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gpahmogmc.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gbljxirmi.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/goyxxbkqx.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gqfartlyy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gxcmdhfxq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gwwghpmqs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/getwekoae.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gdqwlqxwn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gfhscdvea.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gbigjyseq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gvieixhvq.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gxgjcppfd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gcosvbmcu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/grwpbkryd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gjqtspaqc.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gqiuomxba.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gpkdywsfj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/ggqgwxkgc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gannghlzb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gfpxdrghx.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gaervkxlq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gssnqnnvz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gokdmukkr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gadazvfzt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gpitmhqnt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gizbjfdtb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gultgorgv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gawdsdmbe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gncqiokrr.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/ggiivirej.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gswvfboos.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gmfzhibhw.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gvvojnywp.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gmesfvbmo.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gdtgnzndk.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gjmkakfjf.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gxrnkzrja.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gjltzyabm.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gokwhdcup.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gjvibzuzk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gwqtpbgez.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gmvpnycnp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gxyiquvnn.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gtvgrxzqi.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gbymrplyo.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gpjwyspvz.sHtML


<!-- 参考信息 -->