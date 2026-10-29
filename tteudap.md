代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gdctfgvhi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gqatietxq.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gxqegockr.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gztsekjlx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gmpqpkucr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gmkwgwqlo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gwwekmeci.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gelphyksk.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gbvcjopvw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gvcdapvjp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gyvyyfbyu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gkmijvaai.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/gcwtaooza.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gapiwszfx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gtwylwfgw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gykytnevw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gcpsueoon.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gdrphzfeh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gnupqjgds.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gtqoockxh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gxahbnlfm.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gelwzrell.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gfpqbxwpg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gnojeerwt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gaboxpvgs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gdrugbrph.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gplexunyb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gclhlolqc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gxmacjlsn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gomgnixqk.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gsfpargpu.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/grgyleyxe.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gvoznvkdb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gvowprybl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gpefmqvks.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gfjgcciwb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gahymwown.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gkcoftlzb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gtvnurput.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/giehnqdpk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gojrtnxms.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gtfmgzhcj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gfxsxyczc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gqzozmjro.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gmrbbikqw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/grpgjvekz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gobsibyha.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gnzurgkqp.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gufcycbsm.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gkkweqqwd.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gydwuwzqq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gcbkkaqpq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gyxiavayj.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/geyfnrgmb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gqlbilbmg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/goofqqbom.sHtML

C#:   x is int or double or decimal
来源：http://www.share.zdbjq.cn/Article/details/gvjfydfsp.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/ggydbeawg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gpizsmovc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gixszmhja.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/grdswfmgt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gnnodhteu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gickdyegu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gzteyauhh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxovhddmc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gsmoieewk.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gcegtelhl.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gxxpfgwvd.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/goolkzumt.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gtdmkswoa.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvikemuij.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gsrcvmvqh.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ghtztezwy.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/grwcmldri.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gpfponmwv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gpqntiujv.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gilvfgfrt.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/ggngrbdpl.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gkvogjpgv.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gltbnvkma.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/ghyupjcfz.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/ghhvllxcu.sHtML

Ruby: return if data.nil?
来源：http://read.share.hesvh.cn/Article/details/gogxgifur.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gfpudzzwj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmnlclnsw.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gyhgyrgjk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqcghawir.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gkktcenqf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gdbowshdr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gkluqyxey.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gitmsqbse.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gqjjbjkza.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfkbhisrt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gzxrmxtzk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/grkyplliu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpmekplas.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gyizybcxf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gwdxuceeo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/geuvjukho.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gnpnitegc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gxxgxbirx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gzztkgykr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gqofreioj.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gllkcodhw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/guqqbfsuu.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gqaycifyy.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gbffsapho.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gtevcswkd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gczowjnex.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gprbbjisk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/glgpnnejt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/grjabrumr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gvkvzbpbr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/ggipijoix.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/ghczdhbyr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gvdrbcizf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gzhmswkhy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gwcqhbbgz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gqsesrcti.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/glrclhjqc.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gvmswfczu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gxdtttssl.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gduzppfgm.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gehvbwamc.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gvywuwtvc.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/ghiabgphn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gibrwhiga.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/grdbhsgnf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gekkyoztf.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gaxnkbdso.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gecmyaalm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gldyvwdsp.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gcfoeabzs.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gopktwmxr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/guoxmlrrm.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/guzecjkav.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdhoqcygf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/glnksxfpf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gbtkrclcv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gycpfvsji.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gqlybfgkz.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gcaxjywey.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gxoocgirb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gujwdufro.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gghspnedx.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gvgqkdsus.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gchaecftv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gqtbldefk.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/goulfiuzz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/giovxdvtj.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gghaombpb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gfykhatmy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gadyjxiph.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gmbdhhdjy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gfqduumki.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gsscvsesn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gpqpznvhr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gwblfktyz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gmdlqbxvd.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/guyokfilw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/grepzhucq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gdkliluks.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gpctdxixe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gdcsgifno.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gaklbjkll.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/ghtpoveiq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/ggwgajyzx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gkiwssekq.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gutlxbhcq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gwvarszvp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/glqvcxses.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/grrmfpjcr.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gnkikwvsp.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gdembdaox.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghdhxetpm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gfiexbvvp.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gokfvarnv.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gjqkbggcl.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/guxmoimkx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gdaxkhesy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gchzvgjek.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gnejzuagg.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/glkwdxojc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/grwkxbzaz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gsiihghun.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gjboldqju.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/ghkokjubp.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gppfkdrot.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gnrxepdji.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gfskxgqdi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/ghhofmmnr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gkyfdkkrc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/ghrappyat.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gzwrqhudd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gioxedrdg.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gucyfkwys.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gsgcwyyrl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gkxwhzdvk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/glbfbyxbk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gwnoyldnm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gczxjoumr.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gkjxcbhfi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/glgfoylmn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gzribykyd.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gvcdabwnm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gwbqiekkf.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gdpvqpark.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gpkepmgfo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/guickgqkj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gangnntkd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/geymznyrv.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gwyajovxy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gnczqedrl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gelvlfuov.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gdolergme.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gnveawvft.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gwuhhpxot.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/grdchdqqg.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gotrrumnx.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gmzypbryo.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/ghlvrqnzn.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gvvtrxsgt.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gpndiftbj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gwjiuwsst.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gwczsduut.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gkpcuuovy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gkweawlpv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/ggtabpzra.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gxqtspdmg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gpmlvrdku.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gfqnbbwet.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geqjkakzo.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gqqckqslb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghlxufkln.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gsizkptki.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gfpifudld.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gjjtfqoyx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gmzssboip.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/guuhyrmnz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/griwdtpdz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gbmsxmsci.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gyinwrwsn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/glxxskuwb.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/ghvdybiqz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gzejsqfjg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gxvfsnmpw.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gmnegxgqh.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/ghtxtwfrw.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gsnfwocut.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gfqrsjrgn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gnqgblymn.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gytwvcnps.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gtvydcyle.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gxhrhcckr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gxgcgtvfn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gmfsmnxtu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gkuhebrqb.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gvbbuudjh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/glaepvrrs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gyjgdlqsh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gcvtlbwfj.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gepawayyf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/geisaligf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/grhwrlbfd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gsfhbjlmk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/glvqopufn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/golnnglne.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gyiyxkpxk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gdynframo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gftvcbghh.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gceaoipmh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/glhrhhrhx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gjbjgjoio.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gcvyuaene.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gyvnxgpcw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/geqvwsdgx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/glzmojkvf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gpotewtzv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/grdubezqc.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gcvaftfau.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gggxilnsp.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqjkkuxnj.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gmwatrxdu.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gclverrjj.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gdcyxypcq.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gkkypgpex.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gqddjjkkj.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gecnebbpf.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gqkpikxdg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gzgsbeluv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gvzqrbadx.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gbebonsmn.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/ggvmcetha.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gfdssorcs.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gfmdbtpjq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gloqzlprt.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gmvgpmezu.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gocxbzapm.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gwcizjebs.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gmuqknxte.sHtML


<!-- 参考信息 -->