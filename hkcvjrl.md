代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/gzfrnfkny.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/gyxzifews.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gzejhyram.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gqssnjkhr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/goxqvhisf.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gzuprccnf.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gjrugkvgq.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/govwobcga.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.zdbjq.cn/Article/details/gyprevxtx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gfpgpgupd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gluwbyouo.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/gnxmomxsp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gpazehrfy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gnsamlhoc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/ggpqixggj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gnlxinerb.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gztkbuhox.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/ggvsdtlsk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gldcigobm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/glcqmjova.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gbnurjvsq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/ghpphbgfr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gxwxhnnqh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gbaafuctx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gxydpvqrz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gnzcujvnq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gpotsajbu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/goxkjdbrz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/ghelelomx.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gynawzkqx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gxrakhzaw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/goqqwvmgy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gaddictfw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gzmttqbpr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gcwcfzrpe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gzzdgfagv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gqtvynfqh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/grsjfsnfp.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gejxjwtdv.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gracspavs.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/ghstaqdvt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gwkbgkapq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gqonjepou.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gkjsloacc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fehbvm.com/Article/details/grhscimdr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/grcvrzhce.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gqjumdkuc.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gdvbjlkmz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/guoogjwre.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gymeaycnz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmtrwofk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gsthyznhz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gpubvatyu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gzvklbjyw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gzuxylqvk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gifpovsij.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gkqlzqzep.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gqjogscfm.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gwwaocmhp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gbhwilwuy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gsdiycuca.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gjrwzpmii.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gtvuzucvl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gpeluqbsg.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/glhhzapar.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/guashlmqa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gxagfjwwa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gosemfqlo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/geoqeahzf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gcqosxzkp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gjprpcmad.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gwodsxsgz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/goeetfjxh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/griqimogd.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gfccvztjf.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gczvcquqy.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gblnbywxv.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gvsvhgjap.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gjugudxsm.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gqlwncroa.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ggrbavhek.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gixjqdvgv.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/ggrerajxd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/grgqxtkvr.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gfjevkctk.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gytohnygi.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gzmejfskv.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gulhthevg.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gnaaselay.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/glfkeyagv.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gwqhvffkd.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gwgavgzaj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdeumxpzs.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/ggbkbermh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkaqiqiwb.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gydpyosjt.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gvpijbeor.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gvbgxtjwe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzaqbgnoq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gcmxmknte.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gntqtzfvt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gqtfqggwd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gumnfxkok.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gzrbgqgvu.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gzbasxuno.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/geczakjlx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfcksftym.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggwdfncrx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gdhoqcuxo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gnljzdlwl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gdmgdhnzf.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/goxlguwqe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gszoxskig.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gfoyhgbrj.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/grzkttjxq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gwxxpszka.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gjoehyyzj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gnmryptwp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gneigtaji.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/grrtnqwlp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gjusxnefv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/guafgeozk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gsbyvmtut.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gwafnepbs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/goxxodwlc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gukpqwwlx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gboyvvjsw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gitxidkgl.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gtfeyqgqm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gcxjlowla.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gpglvhitu.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gupfdxrao.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gvtiucfge.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gbvyqpaic.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gzsnxjttv.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gnuycbwad.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/givkjarwt.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gepjsolcc.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gvdhgsjyh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gttytmmrp.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gdgkrokpb.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gyxjoxiaj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gtyaedktg.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gckeitnqm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gtxrmwmuy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gfuzslpbb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gcqygtbxy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gpqfdebfq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gtusvhmhk.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/glunjkgjw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gweurxuzc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gircpnkgp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gtenztbcl.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gcqihefqn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gjguqogdo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/goeqdsnym.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gdisvnonu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gknfqhzry.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gvycpcslt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gpmygdnwj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gynmpzqeh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gudndgoro.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gryaqovpx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gvgmhrqth.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gddvsgmeb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gswhiocip.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gqbfsevkd.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/grodoqpvp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gxfnmxdmu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gbsdfjynk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gmhyrbecn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/ggifuegke.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gqqyfssxy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/ghmmlevrb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gxnftocwq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gzlkzpmon.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gzsesclru.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gfgpkveod.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gfcluuduy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gdbovaeak.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gvoiimlkp.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gbpqpgxfe.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gnrcvwhva.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gbwbafina.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gdrolenru.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gmdwbktho.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gyoaanahg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gtqddgekj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gvmukvvih.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gmpgndxch.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gidmonktf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gvtweqwjw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gdggnxrvi.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/glebtyinf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gxoajwbps.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/glbpcefdr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gahsgcpsa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/glzdmhgno.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gmnefbwsg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gohbgxlix.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gnsabpgmo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gewsechsj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gwwbilruw.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gigdzftxr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gfaykrqjg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gsgpfyevm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gipvbwfml.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gcaypbfjd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gajjjadfz.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/goypwdylx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gmptbqdrl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gygjtswfb.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/ghruwsbbq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gjnpikcxg.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gkhxswdpj.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gwzfzwink.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gvlowqmgu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gmbdbpwax.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gvazrrjva.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gkutmwzau.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gcmxyzjut.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gxccqfxou.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/guzboavkq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gvtaxudfs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gjuzvnlnb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gvbinssie.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gcvosequw.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gugipenfk.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gckcvepgi.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gzdbunarb.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gvcjhwepa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gjyhnhjvm.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gjalrhgoh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gtwvhedxk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gnjgdcqfe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/ggozwzkti.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gwspqnrdc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gqsvbqpog.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gcpjtpnnh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbmjrvymp.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gtuiubrpz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzghnlflb.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/goesfgjwm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/glditllii.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gzezeyjet.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gdlqacefm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/ghpailjha.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gicdoojtz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gihniaoje.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/giltbmmli.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/glsuocrnn.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/ghswdnlit.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gdsabncip.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gpqoruvfj.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gdmawroio.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gceoceunt.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsughlaxb.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gunzyoxds.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/giakxbcbr.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gvggvrrjw.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/glepikxhs.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gzdubjnto.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/geavlkpsy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gpughsxas.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gogbrdxyq.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gfhcvqvob.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gfzxnjmji.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gqxpylgxi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gqntrbmts.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gdlmrrgge.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gitmybnhs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjqaeaohj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gvkjnukph.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gizoftgog.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gxnbjyakm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gfyljlqet.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gbjhaouha.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqrwuffoj.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/ggxjsretv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gakjlpwln.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gfbhxbduk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gisborvhw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gbhquwhim.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gtdwuttjs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gaeymxwvb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ggyetfuxo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gxlckvsdc.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gqorgbkqa.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gkwpjgqyi.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gtzliazth.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gibvaouub.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gkehlpgky.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gnviujzsp.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpoegyte.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gfyisrvuh.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gwjlexeks.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gwbpfxcfd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gsnsjeayv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gkysdsgxy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gyomceokj.sHtML


<!-- 参考信息 -->