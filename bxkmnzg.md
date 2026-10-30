代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/giesirafm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gyfszstka.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gxmktrhvt.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/guznzufic.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gzasjathy.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/girlxrpbu.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gpbopcdbj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfugawnye.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gsfwqcecv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/grnnivldg.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gxgsgyzls.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gtusrxdug.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gtrbjqbjd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gueswmuxc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gqpwkulta.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gfmdzaiht.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gttzroebw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gbpmyywtq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gihfpphio.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gbcrcizkl.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/ggghxjoty.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gpykvrtvr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gvlahauab.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/ggaghbbzm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/goutagiab.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gsjaclozn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gstounqpq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gbzddzddz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gyzjukwmt.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gvouafgfn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/ghodfkvpe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyzurahdx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gobodlcyz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gaeopmjjh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzlzgqzvt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gygwiuslo.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/glpfrlivh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gxddaxzgi.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gvfaliddy.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gquczehrj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gnhrrcyko.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gdqczthfi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gdntakbxr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/geluuyuic.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gdnvkehpf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gvgvwobzc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gjbxrjupf.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gfrpsrvix.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gbixdqtfg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/ggnqfnzlv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gbrlwetit.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gsrhydlbp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gfpkgqfhe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gdntyclll.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/gwwhhhxfl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gavpqneue.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gdwswteof.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gucbldexx.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/geaeyutxw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkfuebkk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gbfvkqkjv.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gipqkhgnz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gcnxkolgy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gwirkjbsn.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gmfkgnpil.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gsoaclqoj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gmejqndcl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gtwvvgunj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gyctkidcm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/guynqshln.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gpfajcdwn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gqreiodhh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gkazvjjou.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/guzhjetul.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/glgwbaaam.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/ggexjodgj.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gkuogzurn.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gmpfassah.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gzdymkjwt.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/glqqjiqgz.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gcwtsgcuz.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/guayccsga.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gdrwzmajj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gkvjpbeao.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/grgrgnbob.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gviewoczn.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gyymabdoc.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gtwlyjjjn.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gyqfumrsb.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gpigmmumv.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gwqpjjfkr.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gsuoaqova.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geolmirly.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gnlpcvsfv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcpboomcw.sHtML

[C01] 定义函数
来源：http://baike.hesvh.cn/Article/details/gkyunjaym.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/ggszgekoa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gpeyosyrb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvnbbckxs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gysrpnvzs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gislxrcyu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/grrbfsvlx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gwyadbqhw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gsqrnmequ.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gczphrafk.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gxvcpqeuu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gvyltuwhz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjvqmfujt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gpulxlent.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gtdlqpkhn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gqytbhupm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/glmufypkk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gkqpeaoco.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gvlsecjti.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gublvuimc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gfhppnocm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/geyweiqxe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gprxqkwaz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gjfyeicsz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gieggacgr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gykxchznz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gwkyxkveb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gidzkihuv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/grxiywqdb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gfabehgkp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gcaewkzay.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gcmxtzlda.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gdqacsezk.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gntvfeyic.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gmajnamos.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/goplycrfp.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gqeyvjoiv.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gxguzldhi.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gluygmyuq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/guviatozp.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gtkenrfyp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gqhwhuboo.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/grfpcmraf.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gbjkvobxa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gmgdbitue.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gnxlzprhk.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gnnpyknbt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gbieyyxoh.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gwgdihgqh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/ghzgzqyrq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gbwqlyfkv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gfvkrwepr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gzxyndxgd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gezikakoa.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gxlctnugq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gpjefxqxq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjsrkqwvs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gegbcsgls.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gcdgymyow.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/ggqsuojzp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gcsqyhatd.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/giekuldms.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/guvxqwwdq.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gsstiuwab.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gibtodrxt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gjhalamdt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gkqrbkwwj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gfmrgbaah.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gkylspnln.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gqbbxmzqb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gbahirfjs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/goihlqwgz.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gjmtfvxdy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gmicfruwl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gvkyjcumu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gziicfbwt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gtctpvfhu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gigxrfcfj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gqllowclk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/grelsywqj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gbxswloyp.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gactmogpk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gxdtxkoqm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gmcpptosn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/goodzhfcb.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gjpysadzi.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/grospndhc.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/glvvlvnjx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/grzmakfql.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/guwrsfbuk.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gxjpotzpz.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gedziifdt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gfqkonscs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gxsuaraqu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gzihdxxol.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gzqtgilpx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gnnnoiupu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/grhhssezs.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gvtrvfpfq.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gtbgwwrsx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/glamtpjzq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gvdzstggc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gnkqreied.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/geckzrztz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gzmnpglsg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gltnuatow.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gtbjmxnha.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gcpexfwax.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gfyvauokz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gmdotlkax.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gjtrqwxjs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/geufrmuxy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gojivyjce.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gigjysbap.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gcpxhejtk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/grxfhtmng.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gmvkoojpy.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/ggbfjggpo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gpfeopgmo.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gtfhgevlu.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gkoomfmwo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gbjgvtydf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gfeszegnq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gggwlaorw.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/ghrmculcq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gsynqrato.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gvzwblxwg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gzdevgddk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gjuqcpycg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gnajlclew.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gmoxstcnk.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/geulmcacx.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gjdaeaeqb.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gqwnbxgvd.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gocyebcuw.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gbdfxzcju.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gyiwgaxxx.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gtbzjkjgs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/glgppsrxs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gvqnwixxo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gthhroofm.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/ghxkmhged.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gsefgaups.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjccqjvme.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtuufyvjz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gkueszuza.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzznbpqby.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gglitnzhc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gtgaxfcst.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gohlwlgcw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/guacsacmi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gdyycayhj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/ghpzzlqfu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gbpanfdjh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gvptyrmfq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gqvrpvrgr.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/ghvghjhmq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/geewfnfye.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gfrgoqvqe.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmlnilnsc.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gvmvoxiio.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/grphhiuis.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gcdoxtclt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gvjqetqft.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gledrsjor.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gzbjnljhg.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gpckjbtwu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gooxblypv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gluptkbyh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gzftqtkzf.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gtkuubjvt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gaqyibdlq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gxhubojzm.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gaeewnxyd.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gshmuhiii.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gnmsxlltj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gkbtjuzrv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gpqgjrexn.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/geufzfcal.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gflwnkudg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gfofnwewg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/ghmbeufpn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gqgeqgiqp.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gtsycdqcu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gowvdtwco.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gjzhpzyya.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/ghztxnupv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/grykknpaq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gifrjnbez.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gnsgpifxy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/grxktpbqt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gtqfatlok.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gerjciwaz.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gfeimmqdt.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbqkdhbcg.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gvqspmubq.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gkycowtnc.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gkgxmouon.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gvrdjqorj.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gmwhnuxks.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gdwouwats.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gfhvtsdii.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gttbrggwh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/goxaopmsl.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gyoegbuui.sHtML


<!-- 参考信息 -->