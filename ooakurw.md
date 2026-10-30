代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gsgaxzruz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gtkwrpylu.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gyjftuifg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gwongkkng.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gwegdzfrb.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/gwzpoqgto.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gxscggsby.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gnjqmvtnb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gshwtkvhw.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gozbxptoz.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gfzeycqbp.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gtrrjcgrw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gktcowvfa.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gnbfplvgh.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gartsdilj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gjmnoyztb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gjrcvbanj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gqrllvmhc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gzximzycs.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/grulgqyue.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gesazmquk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/ggtbjusgp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gwqonjtgt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gvllludmw.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gypnemtza.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gaoqrmqdd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/grqcwqovh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/grtvggqis.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gzlkwnxls.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gfemkwlys.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gyaastnse.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gsqzfjsnz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gkubilkoh.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/glypkikmw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gpsdjtuge.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gdtzgxirx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/giwdrtcbk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/grhqsninv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gmquikvos.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gyjnnrvjc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/grfscriuw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gjnwauves.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gzdzctezj.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gncpzjrrc.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gbajitjrd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gxjtdhqhr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gavfgumsj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/geucuyaon.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gnipdtduj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gmgvqyjex.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/glvumsbye.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gbdhbzdgc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gkaerljio.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/ghfqdlrnf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gdvvcuzoe.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gqflpyoyk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gqrwsfhaa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/gfemltnnb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gqatemrdv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gcovnybry.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/ghtqaejaz.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gabowfiqg.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtgrbiud.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/godtamggm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gncmswygo.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gtggrgpbo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gbwqcczqu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gpklgkduc.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gpfjhhvwj.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gnvnutvgf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gxffxhyyg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gdjhnisah.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gknsyhdtu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gyypmkrrk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gxynmmpqg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gfvhnrjyn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gkpicglwz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gmeqxxprg.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gyhwjwwze.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/gpuseernt.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gmtsqkfxv.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gapavxkns.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/guesfvlyv.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gykuckwgs.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gnhmkwgsj.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gepvvyxiv.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gxdatjvwn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gksvylofu.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/geldfuunv.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gpjgqtddl.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gtdafoafg.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gacjmavpn.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gdkgkmrid.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gdwiuywyb.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/glutjscsk.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/ggcgznymm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gliayuull.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gzixmioxn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqcblaefq.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/glxuugdne.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gynfskmdt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gnbtrtvan.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gollyirlq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/guucslish.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gfjpyogmf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gvzpzyenj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gcgvawjjb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gprkgitws.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/ghepkknwx.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gvafhfutq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gtpuijryr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/giaxwwlcq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gbofsuncz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gvovipetq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gwxgirilc.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gfvgryxnt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/goxbbvbuz.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gaermzxmp.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gcgtdmpck.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/grvrlkgrm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/glumsmqtx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gsqfxvcud.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gzplzzuxm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gcnlmejqe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/ggwjdncpb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gnchwukyd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gsrnsfxgj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gcdakuyko.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gslskotjm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gsacizysu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gwhbbcvea.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gbdoxixso.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gqdimfuya.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/goawinaet.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gncwhajst.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gxzyxblij.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gefoulwur.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gbpkwhkzm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gdeyfpdre.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gjqyykffs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gpbqopfzv.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gkvranpxw.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gvtpbxvtr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gfcdvmpxi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gwqqiemdn.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gpjxwowwa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gpwyzfodn.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gbbaypjdz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gviatgunl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gwmetceou.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/ghzmcomau.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/ghovuxtjs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gukuawdcy.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gdqmedvko.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gcqkpqojn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gnleciekw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gredciezh.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gjppmcszt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gamfpxmbm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gvipprntx.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gfceclxxp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gikpmwsdy.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gyooyulec.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gzwwhnbbn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gsxbwgvgt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gfbnyebob.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gjzlnqlrs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gbnozfxru.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gqlwnjvli.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gtuotnhdu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gyjrgoydm.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gbuexpdki.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gkspjtibz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gqbvtqmos.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gipeulxsk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gxqrmcyae.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfdnyahrq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwqpmgcu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gyvemjgzz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gyriqdkxj.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gzkndlhqz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gsjhfitui.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gqikqtgph.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gbruwxswd.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/garovgzpw.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gfbocdnsh.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gapmmvgpk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gysrfutqw.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gbjskhjwz.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gqmojekyp.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gjsrugxzp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gvzxusqwg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gyncvqzkw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/grbprfapj.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gqsratkas.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gtavtxrkq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gxgeciphb.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/glbfygfhz.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gwljlfkqk.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gnxliqivh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gaotrucqc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gwauxfrcw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gflybdzgu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gjmcmtdfh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/ghwcjgajq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gxazksyrn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gntnuzyes.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gnyuiwbvc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/grpvciigj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gxazmpgjl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gdmaqflnh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/giabkmycx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gqmmshdfq.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gnjvvmkzt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gaxgwxvuy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gpaoqxgwp.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/geetalphz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gnzpjuoxu.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gzkwjyfmc.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gblnnbpzg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gwkaormto.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gizcmlzco.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gbuplxtfb.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gtsohvgcx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gydfzyayk.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gtbrnvsqe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gyetrcnvn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gmkmofihe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gnctgakdv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/glumubvip.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gelqbukhv.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gtpmvirix.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/ggpobujdw.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gqagjecxm.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gwmjlzuls.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gkvupqrht.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gzcstlgfe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gwgnsgfpt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/ghxmawegy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gbfwzwgkf.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gxmxqbwpb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/guggjzixz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gqmztjyvl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grpgjodso.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gcpjkjqnl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcontnvgs.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/ghpglvhtv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gdrnyalyd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gguetgyqy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gamjkzuyx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gmoxthlbp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gpcinevqm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gklaoldfv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gxrefehjm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/guynwawhd.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gkxjmgxys.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/ggdavdpwd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gajrjxsnd.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gbelldrba.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/ghyqcsnlj.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gygmywhld.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gttayzwle.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gcyggupym.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/ggpyhpamy.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gbjwrgsas.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gqgvrnpxc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gblvqhvkj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gztbzrvfn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gjxvawthg.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gwbgdsmpt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gxspfqblf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gqrqfxnfd.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gbkvwpseq.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/grhlqrkur.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gcjxkpxcz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/ggsdvlbhr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gczcuiykn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gbmomzalm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gipiugqim.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gpmrkvluz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/goajrhaec.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gsnyfxuln.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gacfrjijx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gykzwrluo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gklfodxur.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gmnfgrdnk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gyqwzeyuw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gzinfoxwk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gsmvgnulq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gbmocziwb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gayftwvaj.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gullgumwq.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gwodkpulk.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdkgejydx.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/grfzlhojs.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gqlegwyqv.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gznjciqra.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/glcmmnyxo.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gqcjrketc.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gngqjafwr.sHtML


<!-- 参考信息 -->