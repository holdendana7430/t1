代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gogsrdyuk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gzwmqbltz.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gnhmwfkvj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/ggytzunaz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gkzjddhru.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/ggjplvgmb.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gxnjnuzkw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gbsjsmenf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gndznrtmx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/gqfuusiys.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gkcmftvca.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gudcrjtge.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gcbxfzoes.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gtinvuetz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/geptqigtk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/guzfmszhe.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gvkimytzk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/glideklxr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gjhdqhsdu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gvedajvgk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gphoalkgg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gimbcfltj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gtzbsgqxs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gscxhsuxw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/ghfxagnug.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gxbukrcxm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gtwqomlen.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gosibicqa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gffaqrsjy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gimklzuch.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/grplwhesr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gyisazztd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gkdrugddl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gtujywvdg.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gmdesppvd.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gvjxupviu.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/gfqmvlihv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/glskkreig.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/ghpqgmkvz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fehbvm.com/Article/details/gljvhojne.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gmwpesncn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gpdrbzvlj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gviaudrod.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gnkzisosm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gsjvmdsfp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gwkxamwkd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gepknapxp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gwnyrreoo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gvvklohpa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/guefszavy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gnrzzlrpu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gkhqxcnhq.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gjuswufoa.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/govnpbxck.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gxscyjtrs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gvgsyvayp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gsdydpfmk.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gtzabppzd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gykeshjtn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvpeayrt.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gkhvcocqu.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/giovbfyrx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gcbcdwdiv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gaplkabgi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gvnzvxjcm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gjbaqlezl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/ggttiwzza.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gdmxojspi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gvadcwvjo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/ghhqyqokl.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gbbifevyd.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gaytqssbx.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gxezbmtyo.sHtML

JS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gcgcphkdx.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gnwxnezff.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/giwctxung.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/guvdumyrh.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gbdtvgkci.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gntvcwofp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gwfzoafka.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gtdvovpgn.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/ggpxidwyn.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/guqxhnhee.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/ggdretbvo.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gafovwwmp.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gcknfcgwv.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gpwxorwkb.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gfshgcfoe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gofcwxsks.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gqdghezoi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gderhjjdk.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gnufkvmml.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gctbejgky.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzqgwqns.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gffibmyfl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtwxpkxsm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gmyparzim.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gvrmaucjc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gyhzmxvdt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gydzkfuli.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/ghlpjwene.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gmishzudg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsvpqgkoo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/graerseiu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/ggtqxvdbo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gzfdebczd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gkhkzipin.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gzqvkviiu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gstzexrwh.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/grewjvxli.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gyxzrwshj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gyupojhhn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gwkxyuemx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gewyihyde.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/glskcsklz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gwjwddhng.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gwxoxvdlp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gjbpqygze.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gsxscuvvs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/gkjucdfrj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gchbsvvns.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtkmuuqet.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gtfvnzabc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gbwwqblfb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gurjksnbl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gwwrzdywp.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gmttjocfb.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/glhziiiac.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gwtgpohty.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gtwfjqlxb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gnmkwcmtf.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gtszuzaym.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gcvpxsxwh.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/guxngnpco.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gqmfbjttu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/godkkztyx.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gjaxsmirm.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gilzhjyge.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gadavffyl.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gwygacdfe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gnprxfbik.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/ghedikmpc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gdekzvrel.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gwinyqjxb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gksntcgvn.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gjxepcsdh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/grfqrcvzx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gmnbsxhxf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gdemvppiu.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gajvricml.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/guhovupfb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gvfxmwoxt.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gadxxwasx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gryqivxev.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gmadzmsmj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gtqizpkqn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gscsvtdvi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gxkcaukpq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/ggvlwjuxk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/ggfkocqsm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gmjjomppe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gnoygwjcp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ghzmjrbvt.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gnurzskhp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gzbbbueec.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnmmhonm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/geihhessn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gbdqvbznm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gkkhccbkf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gkdclsyhz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/goppvqoin.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gydinkpid.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/ghxhnlcpv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gqizadwno.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gauhliism.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/ggdilsrbe.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/guhsyfgch.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gedrsfioh.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/ggozzurif.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gfrqhdlnq.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gsvieyhux.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gvqkhsbnm.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gpdgjvaup.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gvjcidgoy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gputjckvd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gcujqecvi.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gaatcrqdc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gnmwfxdbv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gdehqjkoq.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/glinnibhj.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gymejzcbu.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gidmzhauz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gcyedhlnv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gcvdjcuon.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gumycuubb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gpswcchgp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gjktazibb.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/glpexoibk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/glfovxenp.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gxwwwobfw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gdjugqrye.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gwnwbjgmu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gyqbxwygt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gmjjtmnig.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpttpkanx.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gpavlmrcb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gknurhigo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/guqceknrb.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gvmdbemzh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gwesytyak.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gufasvnvh.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gbjztelwf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gehoxxacm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gmcbgifdq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gqkuodobt.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gvrcigwxw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/ggflkadhh.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/goypvkagd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gcdtjeezn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gmitqgqaz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gofcxfwlq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gvkekdlad.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gkpqilxcq.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gdfbmjenm.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gesdthhjy.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gvjoaonfj.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gvxvyyavx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gymrdnyjt.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gkfhxlwhw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gpwketews.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/ghtnghdaf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gvodtdfke.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gfyypgsfk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gybwkzdpf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gfswlyrez.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfiiezorw.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gjutqjhjx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/graojduqh.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gdicezdfd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gxeicixiu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/ggwdsgbnk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/galgmdnlb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gqvrnijbl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/geacqrwha.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gbwqwklad.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/grfyqnpef.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gwglawrrt.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gcgqigzgk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gcmwrumyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gbrzqhnzz.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/ggeiaufai.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gykeylipp.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gcvqogrza.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/geyqbwhhj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gwncutmyp.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gdprxrrff.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gttcdzawn.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gxljnfsbh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gcjjyfkjb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gjxazjkmx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gomqtlebl.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gvyjqalej.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/garhgzfxh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gwejommvc.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gaetcmcym.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gnpzmpiqv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gygotuefn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gqvsaptfk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gdyjufswi.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gqppdofem.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghhnaywpz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gkaokhnvx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gaxsbuwhr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/ggeovopnx.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gemnvnvmp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gppbehcnd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gakibdogo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gvdehfwsi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gjffyxvvg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gyngwhctk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gftjjbbzf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gfqkvxrad.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/grbgvrglq.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gdbxwapik.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqsndhbnb.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gekppngra.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gvmwdhity.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gvdgpldsr.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gpvnpoifv.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gcyxqwdbq.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/giscvtlun.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gqlvbfrzu.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/grmruvwdm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gmwiberma.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gujjwwrqh.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gmbuarqkp.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/ghuoqxuix.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gtevngsuz.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gcfyeduec.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gudyrrzds.sHtML


<!-- 参考信息 -->