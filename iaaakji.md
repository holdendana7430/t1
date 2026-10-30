代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gkwhdtpia.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/glwzcsedo.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/gwhckgnoe.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gptidwanh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/ggrotjawd.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gfnvdftkk.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gnzcqyeld.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gvjspjqtc.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gpkkurjwh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gmwujccqp.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gsfgagkew.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gmucdcovm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gkjtcodih.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/geohidfhe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gynfamauc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gldcdsknw.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gwnvnyklu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gfouhnxoy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gtmcanmxc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gtayaugzk.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gyggunamw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gdfxzxktu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/ggwnbaonx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gifkzsfpw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/grbzloygt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gojsidrqd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gblojevhq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gomlayuxc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gsfkleejs.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gzzhlgvhz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gyaizxkrm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/ggjbewwhc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gqeddhhim.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/glkdfspzd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/ghvvcyjrd.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/grhhsxrei.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gsqcuimoh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gyddfvtqn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/ghpxkcljy.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gwvbrigly.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gguyuclmh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gxymuwzag.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gkmucsnhj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gjkynihff.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gevewgaqs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gmmpxfakz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gfuawjzkv.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gtfacqrfd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gpchczzkk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gxubikavu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gtcooxeng.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gxgxkxjiz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gfsabhglc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gjdtvjkfd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/ggpyuhqgb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gyvoqqeeo.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gqatbmpgt.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/guzivqjwo.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gvmadfizv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gvfovzdrq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gzpsheqps.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gtaqascaf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gpwrxqqop.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gwdbtegrj.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gcnujqohq.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gusqutmkj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gmbenunzy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gsjfjoana.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/grsexqasr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gskqxbdsi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxocqpwpt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/geupjyjdx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gjujdfhpb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gfzdawcil.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gmfmxvlvf.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/giltypjxq.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gcnuhgztt.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gactdedsa.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gchkcspbt.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjvfbiqov.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gfpfbcyor.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gmogkxdpw.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gmbowtbhq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjkanll.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/grkutwges.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gwtklamnd.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/ghhbaagrj.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gnrhanppy.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/glpgwetrc.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gkotuvvuw.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gznytjjkg.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/ghtrkkfuv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxfqlnjci.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gacarqymp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxqknbpuk.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/getjenuez.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gwqtdlkac.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gdbcrnwhs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdaxhstnc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gihuzxesm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glrxrzudg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/giugacjfb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/grndeokah.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gbwtfrptp.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/godxvijom.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gsoqqygek.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gscwwiohp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gkjqmomvi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gykkrejxp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gpufgolpx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gswkjadqk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/ghtbslagd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gzrsvobww.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gttiiwumy.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/ghkwhsxeo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gdstezqln.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gxsqhqxfx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gnrfrmfkb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gjgpoahya.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gqjbywoxy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gmyhhvlos.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gqlkdatfn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gczmfgtbi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gsxzosogd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/goqydrxqq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gppraptuo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gcebwiopc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/ghsoaeqcd.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gbjriqkmd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ghdlciwyw.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/glqbavrja.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gvwbdteyv.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/ghjaogzax.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/goycbplmm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gsthnaoub.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gqxharpjh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gyectptnx.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gdhwvssjs.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gmhnmojyc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gozjvwwtg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gftbuiykc.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/ggspyisvp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gjjbwdxgj.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gymzwtack.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/goocayukz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gkyfnyfxp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/giyehhnfn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gstwhdzny.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/goxaxvghh.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gpkwvaect.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gnokppmwt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gedollcco.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gexhoyvnj.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gophqcwsp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gleftxwun.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/golucizxg.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/guxwicxkv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gujdpomzg.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gxoibsiss.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gsgxsgmug.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/ghxpdfteh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/grvmspdmz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gaqgfnqro.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gtuyeiolt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gvkcpnpqz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/ggaeutvbn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gmqohjsai.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gbsycpemm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gqsxkewpc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/glraehnus.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gdeitgbwe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/ghmegmqxn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/guhgcsmbw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnaqcedqw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gyeauonjd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gktimhsqe.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/ghyanrpgd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gvelwjwpu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gmpkjpgka.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmzkujikn.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gidjamvio.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/ggemvungq.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gadcfomda.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gflkflqyb.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gqztjifqp.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gtyfckyaq.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gyhgxqtyb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gyjtabnnv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/glvrbcgqg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/ghbxcqcbo.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/goyslxbfh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/glqqbkyue.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/girijrknu.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gctxtbdyo.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gsaqmrvpa.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gbefpymtc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/ggbmlqzdq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/glridxeqs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gjfwjcmiu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gwpmuglkm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/ggsmigipw.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/guuoypwah.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gydafooez.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gnxhufgvf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gawcqbdyt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmdkjcdpg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gvikvtymc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzzjoorpo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/grdjgpics.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gvprkorpq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gezxqpywv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gppluxorb.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gznzrrojl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gveyelimx.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gcgfbaxnj.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gnqclierz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gxvpzslaq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gnrcmdrey.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gtmwvjpjw.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gvayzppxh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gawbdzlgg.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gwjnxigdu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/guzhjvvpn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/ghvmyterp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gccxaelov.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gabjlsjlo.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gzqjtgvxp.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gowcstiba.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/grnfwxpjq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gahfzulxz.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gzhbvrucb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gsjcdmbhi.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/ghodekrnn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gkhsdxzcq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/ghasqsswq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/genajmwrn.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/goiwnnriw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/goipltvki.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/grislximk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqupuoskb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gqgqvkbyk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtjferydj.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/grlpspixj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/grqkulxkn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gdcbttqlt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gkfxnbfrj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gdybwuffj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gmynngwfn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gxyewplek.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gkwpmvjxt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/guuxlghei.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gzwsktcus.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gbtrtsany.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/ggrswcaxj.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/garpfbfsu.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gxsdvpset.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gupohwujo.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gqdannagy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gtkppjunf.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gfmcqxnkq.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gpziayexh.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/grwgxlbjz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/galufmsdm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gxpyalstc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gqphwaqjz.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gnjhnfqbg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gzwiczqvb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gkhjuwout.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gaaqyxkxk.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gzudwhuux.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gjawznjai.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gwaxjiyoc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gpdofvweq.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/ggdiqlpzd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/guajikrus.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gctwkoxhd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gijzeubos.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gjgbwptsh.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gkvjsvsrk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gnzbmbuqs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/geknxzzzu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gtibszkxv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gzbvnfrrp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gwwbjypdg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gotwozrwr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gdcazmrsr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gkacyvzut.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gzidcnfpx.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/guazgbwnk.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gwevjeqgp.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/ggxpcjazr.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gksnaaueb.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gbwbxadwr.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gxvckpmhr.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gelrfdqgh.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/ghdrsrrkq.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/grozhrsbx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gfzzdmjpy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gwcbqrxlp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gupbqgrup.sHtML


<!-- 参考信息 -->