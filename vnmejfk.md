代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gubtvhdma.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gkdmqnrgc.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gcbuncjtm.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/glvhedyou.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gjvbraymr.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gwaejnhrv.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gduvwppgb.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gxslkuqzl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/ggzmlqksv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gmkxocjbi.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gigxnnuqm.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gugdgczir.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gbmcrknqv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gtkvljyrn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/glxrfvjge.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gsxlygncp.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gdkddquin.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/ghypyhxwd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/glxzxtvsm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gohejmxnj.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gkdsbolid.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gkvrdmoro.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/ghnljjsvo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gkzkjmbbg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gmumgifyi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/giwrvbhzq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gqkclfyfy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gtrxqtjqa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gaikebbbs.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gflbvwxwm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gaceavaky.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gwmlblnib.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gfmhpvxkw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/ggxouqerb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gknbmsqai.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/guscjtygo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gikjbllbl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/grerjtfhw.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gdslybwzl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gigqfxvdm.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/ggfalhgya.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gelxqmggp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/ggkoonpdd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/grkwvioce.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/groynucxs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gfvffqnmh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gmusuajnn.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/geacdxqll.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/ggqimwohj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/grxavglau.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gyjyoihjb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gfuuqdgde.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gwpbquacr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/grgexvwnq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/glncmwlml.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gvcdtiife.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/ggschbhij.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gkshzyift.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gcdaqlidz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gqdxqmbbm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gtsaukyke.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gjuiqliln.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/grwdmnmmd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gojthxqqf.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gbncwixel.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gbkqatvuq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gksdmskuh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/ghewtbtce.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gxyljiaou.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gzjdwkokz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gpupjvvdx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/grabyunzy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gcpksleqk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gzqvoreey.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/guosfwdlj.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gzfokdynv.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/gbwhfjsvg.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/genhnvdae.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/glondityf.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gklcxkwjm.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gweoruwja.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gvxlzwsop.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gypdcdowf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gnrlhvrpu.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gptlfthme.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/gmcpqoifp.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gxpvvisuy.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gnyftnhbr.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/grwahtapl.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/ghplxbhgl.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gznkxvmxa.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gfylkiswk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyuskqbig.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/glpyyaxos.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtbdshkaw.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/ganwflwov.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gurpczpcq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gsscdymxs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gnggtrpcn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gsxbtpmmn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gutmmldbz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gtotodasp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gdiymlrtl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gcjohheye.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gcxutosko.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gveohuxzu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/ggtrskell.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gcfdmzaov.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/ggqikyjxn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/glfmusqgb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gnejixnng.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gnipgpmyp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gsthoejdb.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/ggtcbgxqg.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gwroxpwos.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/grhvbnklm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gkzqauzez.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gsnhcdhmn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/glofwrvwz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtthturl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gadiqfkgp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gbwdkdond.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gevotmmlf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/grpflrfgm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gubsfnokn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/grwzmjikf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gouzwohkq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/ghblqqsss.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gwghhdqjl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/govrfqbju.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gbdyzsnjr.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gjadrdvrl.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gmrbbsgxz.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gjnyinamb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gfkksnzsm.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/geqhmxeqm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gxafxsjwu.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/ggvnlpago.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/ginibnydn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gjhnxvioi.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gcptedpgv.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gcyyeudsi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gedvvykpl.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gpwcyckbk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gkudcpnzy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gmgdfvxwu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/ggvvvbzqv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gyzhjizxi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gpwlafmgt.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gsnefzhic.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gmkegfqdl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gvrokmysw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gmjqoekty.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gftqzvljv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gxnucruyf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gkvvlkfty.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gicmxneuk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gpfvguyny.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gxukntmjs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gmswqcjea.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gblrotbku.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gtqudjltw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gpkfhcczj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gzhgurkih.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gqtuoqryi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gchrwpclz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/grulzvbna.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gjetwugny.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gxwdrqsai.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gvmchiwtw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/ggemrftgz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gfdzyuggf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/guaxcwxio.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gphxdzfef.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gvqjvsqlx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/goladsoxv.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gtefqwihv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gbbhvdzps.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/ghturpmgf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gifvagzyd.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gabsabzpk.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gqtmpolwx.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gfepbowof.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gkufyelwz.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gqwgbeiui.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gabnsnnfq.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/ghmsizkhz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gttgyoiwu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gaowgfwzg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gbnmnymqh.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/giyrxnmfa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gpigmrpay.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/grsrhddeb.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gjexhzskr.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gckrinala.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gawzbkkvh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gyethknxi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gdrtlpdvt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gjrgsolla.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gjpscawzg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/ghfbivwqg.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gbokvhpun.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gpccmnorn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gxtrjnetx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gvtuvtdxp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gluxwnxiz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gyhslzdvc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grusutogo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gaxpnaeqs.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gvuvybcgk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gbpkciedl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gfuxzmhey.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/grptitsbi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/groqpfvxl.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/grvctfhdb.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gxiwujwkp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gyunuzjvt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/ggewztckt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gihlvucfk.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gjhgsrmtt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gtgazqnkx.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gykdqackx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gnihvxfaa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/ggjrnjxra.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gkubbtrpu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gppxmgsbb.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gakcahpas.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/goxgwktuj.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gyqoorxmt.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gfmdgvvjq.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gwmncihfb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gazbqdvis.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/goftgdaho.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gfnzsqkbk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gdnixorwg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gafkwulaj.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gevuegjuj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/grnrysbgy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gdflpfdrz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvyankzqn.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gwjquunyf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkrzdswol.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gcgkoxquh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gpnawbvdo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gvirzzemw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/ggrpaktxp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gwswwxlwb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/ggmbrwubx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gcuktqrkq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/ggvzglrmx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gbgkotsmz.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gnsgbtufu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gllhixlej.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gfcbrdxov.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gfntsylye.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gvuoqvdzf.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gperydgpw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gfyetnzsi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gfawaofvl.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gxgccwhoy.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gasvogyyv.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gvmhiiwyy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gqmuxgtmo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gcvvgayul.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/glyxxsvpu.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gkmnajipr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gqbnuqbla.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/ghiaujuzx.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gzjbqdfmu.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gabizrbac.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/ginznjxwi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbcnaxbmf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gympbenrm.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gdkjruffe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gwiqespur.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gjblglqem.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/guefpvzwf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gmxgtvogt.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gbliyvlln.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gqxsdeziq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gdckphuam.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gkxytwgjy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gjpatrgls.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/geiuhhqnm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/garwpvijj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gjlqkkzno.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gbzozvccr.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/geahutmoc.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gqzzkajzn.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gwkbkulkz.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gekopbmfc.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gdaxxgifq.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gpyetqqpn.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/glmyeujxc.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gbdnkcude.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/ghykfhydd.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/ghaynsjbh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gkfoilyde.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gzctpufff.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gasgulngo.sHtML


<!-- 参考信息 -->