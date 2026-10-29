代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/graapynwg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/goqyfbaby.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gqpukpokc.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gnpmcnkse.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gtymbbepn.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/ggjkxxeoa.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gvjkyjbpi.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gkkjvupqt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gjcirzjkk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gbdxlhewm.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gpcndlbco.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gcaoonnwd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.fehbvm.com/Article/details/gluoaiybn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/ghbvxeuqe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gbcxobpce.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gmerwefjr.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gxkionlll.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gokhifvur.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/giszogkxj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gxkrksxfn.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gdpxdjgqp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gpegotlka.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gaubcyjvg.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gieuwrfxz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gxqlfzpqv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gohzidlyl.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/ggrlbpbhp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gplageamg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gwhbwxdxa.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/glmwqyfza.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gusnhbbsn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gfauadmnv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gdjgfbwen.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/giymzlubm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/gpzinmnlt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gmuwyohub.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gotwepxty.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gvegfolkx.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gisfghcod.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gxqgqxuqi.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/grgmwgvxs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gqvkyamxi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gkrcztgiv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gkycftzdu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gybhehxjl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gayhlvmia.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gfkyzwkpy.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gsniucpyt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/ggwrgxhze.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/ghbyjjvbh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gveobioej.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gylxyqifn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/grtfsztki.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gkxzslprd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/glbqwamyj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/ghqmmzlrm.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gltkhwlzz.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gufnqpbzb.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gimwioqoy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gfybqnzue.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmajwztmt.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gipqkyuhd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gllgdqflt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gdodkyaru.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gzooztpyn.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gssuqmywm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/giduorqcs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gozgxcfae.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/ggxdzxtno.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gbpebmxmz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/giulwujik.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gbitwvexq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gcsmwnupm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gbthgfoir.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gbesnbciv.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gdbrtytqx.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/grurfvygu.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gbzxyydhn.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gtoubrqqo.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/girnicaze.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/godqqgpms.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gsyovqoxp.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/ghomibwns.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gwzptejkn.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gzzthoeaa.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/glmxkasng.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gztolaoyi.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gwwnjanip.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/glgwbjbzk.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gwiajgqba.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/grfpnldwc.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gcebcjpgv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvnosnskc.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/guhhaqbim.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gphngzpij.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gyihlqcse.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gupazccyf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gcigdxotw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmwegftdo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gelhmhhfb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqmyhsmbp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gkaunqcsr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gxcpfakcu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/grvplbhzb.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gpeohwaup.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/gmcoynota.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/geiusayqj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gsanxtrxa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gyhcgxcit.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gfwunqjmv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gcktuggjv.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gucmjbrgt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gmctqnhlj.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gzhnemdqq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gbhcjzoyy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gayoboppb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gazkolxcq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gdlwqcfnu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gdntbykun.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gqiwvsemz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/ggliwilej.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gdtqqefxw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gqyymlkgn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gsyttygsf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gannvvxxe.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvkysyktb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/guwpqbloi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gbslmozpl.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gcyjzvuha.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gmwuawmdd.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gzngajnnn.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/geisdocks.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gzzayalzj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gropondib.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/ghkhilnbh.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gzhasidon.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/goqcknevk.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gwxbrwfkv.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/guslxnixy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gpgciixxk.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gqsxwgnoc.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gbispsipb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/glrvbsacd.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gujbkcrze.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gvayjkwug.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/ghnyydlmm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gusllliua.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gjmytvgto.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/ghiavcpqb.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gkazowlrq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/givvdyjwq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gnkywouuq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gukxnnbmd.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/giexqcawx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gtveiorfy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gzgaasnxm.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/giabkzxbw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gppzxzxxb.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gvdberpmq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/guwzhwuxl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/goqukkwri.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gywgpdmht.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gtevinsqx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gouvclbgq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gurunhjbm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gauaqyclo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gqunhwtvs.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gfdcksowd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gohshsxps.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gfsfgcbov.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gjuzpgqfe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gkyljmxbe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gajyttfaj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gucwbcvmo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/geicmfkpd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gmswlovvn.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/ggiqeemjq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gyvrdtxkb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gbpmadydo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gwmqwzuas.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gixrsbeez.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gdnnpnxrr.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gzbtklixp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gzzphzksg.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gvcrbtfrj.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gwmskpcaz.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gjvlljhyy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gznawhqfn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gmhhuuxfq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gcqhfyhxw.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gmnklrkst.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gashhhubn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gjbbmoyyi.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gwxhbodyp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gvwvmnicj.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gjcmzdhbo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gnhvlzson.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gfjtwuzjd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gjltquhze.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gbsqjkajd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gsfvhalxs.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gclexvjoj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gtsiylapf.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gcthnqdwe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gktkzbplg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gtuqnomnq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gbkzoynqy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gvgdnwiqt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gftsokxnn.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/golspcemp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gqovxozsk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gppflahef.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/grqcgenlo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/ghasnxplt.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gfthbajlb.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gxemlkvjh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/griaonvpo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gfnbixddg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gnbfmyqnj.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gimfoqduc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/glzywjqnb.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gbjdjlldh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gjwsrxteb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gvevlpbkb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjkleekwy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gmjqaxwed.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gxyugwcmg.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/ggprsawsa.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gsqbchruh.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gqzczhwds.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gzvdwvalb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gsvznjzmn.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gpvhnasbj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/goqndqbcu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gqyzzdpxy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/ggqizemya.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gwfffttfi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/glfusbnen.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gwputicvs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpdqtujux.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gvceejmov.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcjlblowr.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/goomenvbd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gwxyskamr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gutffoadu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gzwvpqkuh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gyujscety.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gccodallp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gbtpljugf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gtpkoahoz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gnmhmlxtc.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/ggqrayvtq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gdzgeekkx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gdhlcakuh.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gvsngdslt.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gfxowbhzc.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gdfuyakdp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gvfaguprb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gfclgpwqq.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gkvpcqryi.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/glbfkhzdt.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gkwqyibtq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gcxixgfxp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gmcjimzhh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gyiaoxpoc.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gqjrqcchv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gvyafcrtn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkoduwxlh.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gziavilgi.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gnttruyeh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gzbgakaqb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/goomfzoli.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gfyufqcqu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gfgsffvui.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gyeucdpub.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gexmezutm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwweicpvw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/goeytjvuv.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gisomdpim.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/glshqwrao.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/glpdkkpaa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/grzexjrac.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gvviuauxx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/ggpcofndd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gkqbduyio.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/goalskzxf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gaqrocnsx.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gmronmrgz.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gqxqsqucy.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdcimcbj.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gqqznsmgb.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gmskdbgvr.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gkmxqhuuu.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gnzimrwfy.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gbhxdgipq.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gcgdlvexi.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gztaccpvf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gelxlzlet.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gzcooqlgv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gyhjphvgx.sHtML


<!-- 参考信息 -->