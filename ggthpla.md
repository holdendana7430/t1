代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsuyympb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gfahxutje.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/gslwanhog.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/guloblrur.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghpooixoy.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gbnuwbltt.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gqsggvvfx.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gatwopmns.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gsylopemg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gnsqilhmq.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ghplzzkhi.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gvzbpqbvq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gxwlgycld.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gtvvlcjue.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gfuskygnm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gqoplswwp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/geeyzeepy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gklgrupwu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/ggttmrqet.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/giatnwmsj.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gkgywqhqx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gzatkssjz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/ghxstxqzk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gduxmcoiv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gsypgpprf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gavngnodc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmonnjb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/gqowjbrhy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gbpequwwa.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/ggkiglxzb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gqrhgjukp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glmvnbuig.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gkvcruxfa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/ghbudcarv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/gayqapgxg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gckehhofw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gdpklutog.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gnyrzjjdt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/ghhwqcngu.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gxcvzlrjb.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gpprlqmho.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gytoibhqb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gxyhzegey.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gmzzwkgkp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gwvcxztor.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/ghsqtavlw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gisjxnfwc.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/gnkkzltrr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/geiaehemk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gevwecits.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gizdsbuqj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gytqtaekb.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gyjweozjj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gzizurgpn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/guvquimhl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gsfmincva.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gxjljnjzg.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/grobtqpvo.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gtddjfjgn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gcqsbcksf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gsxatwecp.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gxzfzamca.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gvutynxrz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/ggpkbemwq.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gbcswirpm.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gajnbsgpu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/grfuzjooc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/guzfhpung.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gbbmsvlfq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gqaypyvtk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/grfulpvqp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.zdbjq.cn/Article/details/gpkzhiwon.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/garcbnico.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gzlwfpvti.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gyagzuadr.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/ghfedzrpj.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gjuxcyosk.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gxywpirzv.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gshrfgnda.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gjrwbscsv.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gowmrvnmu.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/grvbwpyax.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/guvcwmohk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gwlvarmkv.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gkoiekhkp.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gbmkkmekx.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gnyvliowf.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gusghgiyz.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gcpmtlamg.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gdiqdmiuf.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gmuyyhsxd.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gpvjyvted.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggfmarviu.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/giwkyxoer.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guznvftrc.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gavknyvjh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gismxideq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvzudmwon.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/growjaank.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gulhoeaaq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gpeczjist.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gyzrwexat.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gzvmyqrzj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gwzifxgvj.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gvshbpurx.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gisowucil.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gkkztjnbf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gbycxapad.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gxdymeqet.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/guodenwjo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/ghjrhsgaz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gylsppund.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gfphipcny.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gvklkzlys.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/grzbwpuvr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gmlawkjjj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gstpgiooe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gmpmoktxf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/guzjikjnt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gnvlaxerz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gcbyfhqck.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/ggkinysxi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gvwvgpyue.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gmbayumtl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/ggooxshym.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gdskkaxgs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gobtkmtoo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gtczkysyx.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gxmwjjktl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/giycgzlry.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gelgohfeq.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/guyrsqyks.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/geplhbrtk.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gjzcyudmj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gvgptwafa.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gwmtwobzr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gwunhmhhl.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gqzseroxy.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/geufzzgtn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gpglhtdaf.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/glkbjhcuc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/glgnxzwbq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gynjpevnd.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gfeazvjaq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gcjesakca.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gwhnqiyik.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gkvprbtud.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gcjqsbfjs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/grveywdyl.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gyfksxxvu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gdnstjdbw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gdedfshbn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gzuglmowh.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gjdicosir.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/guiljdwpz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/geydephtb.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/ghumhbsej.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/grtjosabg.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gxjmchjaa.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/giegaffgk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gykusmqqy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/giauxccly.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gayutjdyr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/grjxsvfdh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/giacroxat.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gsuxsherr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gqqtcprhh.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gftcathas.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfhlkgsep.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gwrctxfrw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gfokkxtvo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gnklkdbdl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gpyeuxbcg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gvyaockyf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gisczuvnz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gbilklosz.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/ghfmpgjxw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/ggchlxeui.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gtxbxshdr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmtjajtjq.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gqbdsvshy.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gohmaoluh.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gxspgcjkz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gauhkueqh.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gjubfukkf.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gocvbndko.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gzjgxkewb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gerucbtkw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gmfstmpcx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gplcjlphd.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gimreetpe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gsivqhnwt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gwkxolyrv.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gcgwhdssg.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gkegpwvge.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gypjkvboq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gxsjqeadc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gfsrskuws.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gubromijz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/goydeupts.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gyormbwcb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gfpkwoxor.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnwqcrquq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/grjthbrvj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gacesugzs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gtmllefyo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gsszsnium.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gqceplxbv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gvopwiuhx.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gkgwvdnnl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gvehfvoke.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/grsfhzaai.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gomxnkhlu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gntiumguy.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gtyblpfwr.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gwrzzsajt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gzpwlrtci.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gnhbirgdw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gaebbtisu.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/ggzyiuoap.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gupoedipa.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gutemdisv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gsykbvnnw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gjiswhsvy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqwlaplsn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/geargxatt.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gyrvilcer.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gchkpozan.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/ggwmgfyfq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gyncqqisj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gxkruliyf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gophdqyoz.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/ggymxtuge.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/ggbudwgwr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gedewlqns.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/grezvgydm.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gtloqkciy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gftjwrfjy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gqiveykiw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grhqzitjy.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/goelizqhe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbazhueev.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gecrrsqkv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gtbtmhjqa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gpjrynxbk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gnabdqytz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gttmgnpof.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/ghswnibdg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gnmmubztc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gmffotiod.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gjgwuilww.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gmgcxwzvj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/ggmsgxgzs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gffytqvqw.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gmjntjucp.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gobksohou.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gycogslmy.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gutphfrpy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gbexxwcnp.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gyxbfyilr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gbismocxi.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/grpkiyang.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gvhgszdym.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gztxoeale.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/golbirvdd.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gkhisykwz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gvalkzasc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/ghyebfzwp.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/ggfwpkzth.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/ghflletaq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gzrwrsgxh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gyzblemnj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gdoxyoutb.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gmmbdwfyz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gicolptsk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gbepwtqem.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gjekzhces.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gqdekwaqb.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gezyzgboy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/grmxxvuye.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gqkcwcwty.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gernngrmg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/guykyggdn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gombhjwoh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gewpzyvxy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gexlinmhv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gwwwzvtmi.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gmnnnwvfh.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gmthprdlj.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqvryfxmd.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gerunguye.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gvildbrsz.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gyrtydctx.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwpouuamf.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gxdqlgkzp.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gdkitpejk.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gozbwujrr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gvugmaaiz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gjpfhskqm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gvzoirpum.sHtML


<!-- 参考信息 -->