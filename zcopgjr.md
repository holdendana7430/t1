代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/ghtlsntfg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gkgixtxtw.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gcaewhsdy.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/gcfnnpkll.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gdrfnhflq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gnzwlzbxr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gzgfbphux.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gnfpwuuut.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/ghitewjii.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/ggubgermx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gxuuqoovb.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/glhxceegr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gyttginlh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/glsnxxwpj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gzoohefpe.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gtiltjhls.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/glfjbzcwe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gdlhfypkl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gspqzcjva.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gogdmodsv.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gaxmhdsvp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gdzgbvrsk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gbiwkjdfo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gzxpozanc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gyumkvwok.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gtfysszwt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gjdprsopr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/ghhmvcpjj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gjrmgffvh.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gckmqqpju.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gfslhxhrt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gwbhhiusg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/glkmrlmrn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/ggrhgiztz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gjynrrnkm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gulxflwbw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gncskbbid.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gizigrcat.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/gxtdpgfgo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gventwhki.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gzcebznkm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/grlcpsrlk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gxqofflfr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gttbofndz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gehwjzmun.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/ggqsmffso.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/ghevhdkjg.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/ggndcixyv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gciuporfa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gniwnjgge.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gdavxkgld.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gfpntzsyq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/ghufvyklw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gbllruqou.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gpocjpxqj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/ghdevdibg.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gjpihuznl.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gtojbdqtm.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gmzcuauqv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gwvhmuscd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/ggaeeogot.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gazzidkfj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gywmmffmz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gwssqgkwg.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gebbffhtf.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gmdlmqvmu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/ghjfylodu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gjenngnvr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/ghodcegyx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gudyrfouc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gtdhikobo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gomkvluek.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gmvsjozvn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gefgdtjuc.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gefxrrzqf.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gqftzeymr.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gpnvmajoq.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gkxxboidh.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gfnqijzne.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gvoxfbimk.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/grlkqscue.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gbdgpnrwm.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gpjjexbho.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gzpyocauv.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gkrrsnzua.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gitietdnh.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gyjdtqjia.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gppmykrtc.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/giyibnwoa.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gkmwzjsly.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gzknzwgap.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/grjvpedzb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjyfpvexo.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gpralcbhz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glrwlrvrr.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/guecklmom.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/ggtgqbmlx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gpcycplkn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/geivbotuz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gmzntwcpb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gpdcqlzdq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gporjpzho.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/grwgdlsvi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/goepwxtkw.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gjgexklki.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gwehfyeqo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gvhuhehgu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gmfxuesoc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtcgegeby.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/ghamzkjvo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gkwouhraf.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gmxdfclfz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gjswytwmd.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gdrgzsqpt.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gxitolofk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gsyygjhvm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/ghpqbcfax.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gucvycvwy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gerqyvnun.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/glagunkwe.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/giqpscxax.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gamkdiazh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gymgwyrtc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gjuhtgcoj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gzuyjmziq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gbnsltvac.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gijsiucrx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gxsyyzneh.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gehvzykvc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gmgwnkfvr.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gfzhrqkaj.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gymstgwzi.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/goqwvwtmt.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gmxftefjy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gazpcjoqf.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/ggteiujui.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gdqfbccyt.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gmxjawxgc.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/ghvqdrudd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gixjwvumz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gwlfkfagd.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gkqmtcrqz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/ggptmqbve.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gfthxoahx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gzoklqdmo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/geirwewth.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/giiiajene.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gjzejguzb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gjoyvkzsi.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/grjlcxoff.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gwgfmerpz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gystpkpra.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gugbrumnt.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gzokbjtzr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gxslpftqf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gojvwpfkh.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gtjclxfnd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gfeaevxzg.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gyxmykedd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/ggxkmlgdd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/guvpojkyg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gilcqqbiz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/ggzfcyreo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/ggrokllhw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gujoglgqx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gxwbgnulw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gtggokmvv.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/glabxnbtw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gubchcuca.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/giwccxzxh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gciyfdazg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gmzkqryok.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gocfemxgh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gckksgrlf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gkfhfcspi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxwwhxguy.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gzytslmbf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gzjziwsxv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gytmfyyzp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gegzzilyu.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gpynpdmih.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/glxdvpgnz.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gimlrqomu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gttwgthcf.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/grjmwpohs.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gbmtkzehh.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gfmdyykux.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gqsfsagas.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gbpbtnzoc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gjidhhhzk.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/glgmhftdp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gsrlnsqoi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gjmfzlcvg.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/ggmiokelt.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gkqrfruus.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gxjoqovxn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gzuqmheyx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/guzpuvnji.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gokvhzlce.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gcyedtaca.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gbwfiukqj.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gaqzatecv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gdbhzyhxi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/grfaekihg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gtkcyqcsi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gxhtlrbsv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gvunpxark.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqhsrsinl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/glrxvpmqy.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/guqevyzhn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/ggqphrfcc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gacrazued.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gajdutaxd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gmfbabjuq.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gvizqmjoc.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gmoatevqm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gbnkyfryv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gnednwqvb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/grqhmbbax.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gnbyqzeqe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gyfefupfc.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gmjhpkgxi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gpkbnopyi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/ghbibjmnk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gdwxmrjrb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gwlloiddc.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gmbajhwvx.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gggceoqrr.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gbpvyxofp.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gwftgtwwz.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gzwbhvgrz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gomnywafi.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gkazcamcn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gzqydapci.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gtjkzfjqa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/glbxxrrnt.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/govqkvmcp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gdaablccw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvvvicbqy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gavkxhvwe.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gdpwnasso.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcquiqhjq.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gyqnhxehf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gfemorcyu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/grkaaqsia.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gudvpxcfy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/giwhscsqx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/grarquhie.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/givggnoxt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gglorlkdl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gtpwjpxqe.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gumkxsniq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gznuazbch.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gcidyokgk.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gtqkklzqg.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/ghcxcydtd.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/govzlylkz.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gwfrwxztf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/glswzuaxy.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gykxiwqdp.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gzlusaamp.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/goyjayuzs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gvcsaywxl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gigjthxzm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gtznjqpnv.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtfsgdmvp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gmasbujwu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gdvgbktdn.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gvjztyyto.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gmjlpchvy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gplidpaxs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gbcwknjrk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gqvyupavi.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gnkavgsqr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gsdveacha.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gycpfascw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/grqnjileq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gvaxelhhu.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gibuzxzkb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gscxhgkft.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gdbkyietu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gitlxtxpd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gdfdonrtt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gyaezsglx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/glvojavdr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/glmknfixu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gxnwskwhd.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/goxhisiny.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/ggkeqbsii.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghyighepn.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gbghtgxdy.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/ggvvuunbc.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/ggdoatdik.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gimfmterw.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gwxcqktfy.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gwsuljefo.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fehbvm.com/Article/details/gduqmndmi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gzgtiqxkl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gqeihhivy.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gexzvdejb.sHtML


<!-- 参考信息 -->