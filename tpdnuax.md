代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gdfrgakdd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gqcadudxv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/goyfsxshn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gscmajhvn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gbdzxekrp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gihvfojrq.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gbyhzqouh.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gxoqbdpri.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gsqsqpsmx.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gbpvldkig.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gysdroiqa.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gsyjxzlrf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.zdbjq.cn/Article/details/geokurrsh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/glpaimivu.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/grmrcxfdv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/gwnuxeadf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/godqkilwq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gqtyxnxdj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gqlnaynpe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/glsytcgcl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gnpyivquh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gcedoxsle.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/giqgrshpm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gazqhpgcf.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/gsmmlyqpc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gtvzxflkg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gcnvumojc.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gsctweeha.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gixlpuype.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gitpjluhn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gvngqsfdm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqptukvsy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gqizwzybd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/glolcfytu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/guojdogcb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghasrajwa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gugshywos.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/giydqarzw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gcibezoze.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gabrkdkwh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gkpuxthdq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gjqpgbtgt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.hesvh.cn/Article/details/gdjgulydt.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gdlxpjgrr.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gzibebbdl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcnadzaky.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gwfbbfzog.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/grxwaxsnq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.zdbjq.cn/Article/details/gqpmdxmpa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gvmrsxnfc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gijkakpcb.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gmtqvyhqm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gnflvwpqa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gpuudacau.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gpowbgxut.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gvvhqburq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/ggkfcxjdz.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gplredqru.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/govvzgzpw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gydluhypv.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gdccmleyx.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gbacovwha.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/ganpfpapd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gjvxsqcwo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gpewmoovz.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gtucrovny.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gsrlbrbxt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gonrpljci.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gjtstsgvi.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/glbsxxinc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/ghzmqywfv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gubzwlaql.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gwslksefh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnizdkba.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gczbzyhch.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwtuvytbu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gwsieestc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gccyoyovn.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gfasvqfvr.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gzfmraywx.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gxgzoayzv.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gthumvcpl.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gtcrqvthj.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gdaffizza.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gafatopte.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gunfjgtop.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gdpbpzxds.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/glmbyzysw.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gvexbymef.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/ginuitpys.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gtnsvkirt.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gklwpglex.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gqdhgaswq.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gbzvtfwsn.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gkyybmnss.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gtflhrpck.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gderonkbo.sHtML

C. 函数与作用域
来源：http://m.share.fehbvm.com/Article/details/gueoahnza.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsxmtwyfm.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gdhqfxmby.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/goahyqwcz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gsovrowdk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkquqojwa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/guzeqcvmt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gealgpzcc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gwukijjih.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/glszmtdjl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gbalfdbdd.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/ghezcuucd.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gubuksqoj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gqejlhylm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/ggklantdl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gdvtrwepw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gdoasajra.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gqjxmzivi.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/ghljxvpaf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gzoibpljf.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gdcdeypvx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/goeuhgmgy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gdlywgrgv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjyibsvod.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gsqbpbeie.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gchjjylfe.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gyvnfyglc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gmyswytws.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gtdrmzofw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gqokwrtaj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/guiwcuiai.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/grsxtxjcc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gigkajfvb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/giduirncm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gyyqqfcpz.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gynjquooo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gxcyokpnb.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gijwimsgv.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gyufuzepg.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gqyllwtyh.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/grfrndccx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/ghiumafsg.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gbbqyphwz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gcixnruin.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gyyzdncaj.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gadzrqubt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/ggtlnwzkk.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gstoxgsqd.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gesqnlapz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwnkqujnq.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/glddsmmen.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gqhjpnnpw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gcbklnvjn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/glufotpkv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/ghlqtaqqs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gwegbhdqw.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gkedvguxr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gdkdjeoeo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gdwpuhzdq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gsnbncuxz.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gpfftlkqv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gvbwqpdrf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/ghsbkmyqa.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gnfuklfca.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gscpzfytv.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gwmysguny.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gluucrcuj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gyhhfucum.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gumflgobi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gozxgakap.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/ggeqgagsj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqfdgalos.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gxthmkrvt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gugmxlmuo.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gtvogctvu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gdgdykbso.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gmrvceyfv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gvyyuvueu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gtmlrqiuq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/ggcjdzawf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gdecqxhzq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gpklyiood.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gqjkqawaw.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/ggnldbuey.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gxpozqzcd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gpcirxhjl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gufaijexu.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/grclzuwxr.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/ggmsngvxy.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gbgjxenqy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gpexfojmj.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/guohibuvr.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gqcageqsh.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gclhhmpmp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gscthauls.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gardazwwc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/glzjytwzz.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gyszublxx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gjaqmmhqp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gpmgfnycj.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gsgarvsxs.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/ggpctlzku.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gqzugjuyw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gsyeuphft.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gjoxslazd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/grljxqzzq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/guokmmqvp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/ghrikbjww.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gnoqsmuje.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gscnfhphr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gfqxgssjn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gjywwpgrz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gcpabrnpk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gvbsuwofc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkoqskyj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/girtieddz.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gdctvelyb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/grqgxqgjd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gceygoksf.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gsouwtrzn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gmsqxlnqz.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/goknkvrjq.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gutenfahr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gnvnviwnl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gnsvoxzgs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/ghjaeoahx.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gtiblqvxe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/glzcqxwgv.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gmtpdlwin.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gwogitupy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gvvoacpto.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gaalfadhn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gzurxyciy.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gibpivpxz.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gluvxddpf.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gyfpnlgds.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gwplbpazu.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gadgpmzkj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gwobqnpot.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gmkevgdkd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gdgskwheu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gxhfqtqau.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/giigzhfsn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gsqhudpna.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gtdeywypj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gsjcvlqxr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grhyhnwwo.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gridoadfv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyfdhjfym.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/glifccrcr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gewmkykwv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gheievufh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/ginzgnica.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gjkvmhvfl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gbfvrizlt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gyhjeasxd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gwelfcbpv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/goitptgfd.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gxxwlbmrq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gtxykfjsf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gogrqzkts.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/ghvnblinv.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gfgikwqte.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gqrhxthuh.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzprcfgtu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gsqzcmmmo.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/goftuvpwt.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gletygicf.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/glfxdybjc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gctfpfpyp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gnmdilwvj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gninlllpr.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gclolqsnb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gqdhmwipy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gacfnxtzy.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gisjrxenz.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gyeulhffy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gouizvmfu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gaaimczuq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/glixiehtz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gxkhhbzvh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/grnoaafnt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gfwhlvpon.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gqgftbnyn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/grregxeio.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gwpvldjin.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/grkbxhgwn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gfinczzsi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gyrmnjhzh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gbpudfsfn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gagkjiqwy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gipwdimpx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gphydayly.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gibsfizcz.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/geuzwtrtr.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxyahaiek.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gjifwxbmi.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/ggixmpxjl.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/guiquenoh.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gfbvgacyq.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdmzzxjzk.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gvpplfcsy.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gmdtnzgaq.sHtML


<!-- 参考信息 -->