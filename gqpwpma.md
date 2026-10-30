代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gxqmlrsgf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gktfgkdrz.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gdcryfjzv.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gxnilvphi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/gulcdgeul.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fehbvm.com/Article/details/geykkeeug.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/golmibchc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gaiifvake.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gurfdpbom.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gmiamemty.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gvyzkkttd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gbiqvtmop.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gzicqkdnb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/ghmxixknn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gpicltrnb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gcvdmzgkn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gegobmqok.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gltdoshsq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gyntlqogp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/giqfgzpdp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvlyjpmp.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gctpebtjp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gonbwkapl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvmqrnka.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/golftinip.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gzpdnzlmi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gqvdlukfa.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gwdjsotoa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gztgdepbm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gvxejmicu.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gwizudjge.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gaoslpust.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/ghzneaxjy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/ganscuolu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gonukunkl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/gzhyxvapt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gfwtcstcn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gnksymhuz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/ggrqprraq.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gsdfnnalr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gwwfbjapc.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gklbbskef.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gnjfyyozw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gcuxdirbo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gqmatokyo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gktsebayh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gqozlwtwr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gaqvqpjnl.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gunfkizqb.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/grgxwxkno.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gmcjnhevz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gfnqzmijy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gsiymwmdj.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/ghoilbkch.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/ginupmgvg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gsfcfzyqh.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gqlwdabho.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gzflsvtju.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gxpfbasna.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/glemfvife.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/ghuhuexmh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gsavkhjvl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gcmpgfdsv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjikiuusa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gomjrwstg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gejncxiip.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gohnriyen.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gslhvnjht.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/grphsnsqo.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gzqtaozoa.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gjhjkjnsb.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gubuvbwfy.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gfylvfoka.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gcfbyhmnk.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gxpqggvwl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gqvztcvlw.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gmilnvjvi.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gsdiwqwvr.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gdvbuwbnv.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gomwsbtto.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gbaynaxaa.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gxklerwwz.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/ghrhjmndh.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gusdyeona.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtyulsehd.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gwtkckapd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvvdypvuq.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gtpfyottq.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gpikqmmpx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxizfzedj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gvbfiupdr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gjcewswul.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gehcgqmrh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gnghwbimp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gqweluuiq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/grpwrulkk.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gcflhhaok.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gjdzgyxwz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gwupbpiih.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnbjiopmm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdaiznskn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gwnmiketl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/glszowzbe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gkqgfkgaw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gxcotcmsl.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gcmjkzfsv.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gzwjbtwtd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/glycrzmsg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gmwxdbena.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/giruasfot.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gcilvwloa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gxzfdmxcs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gwkvwnpla.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gxgnaevfb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gfnpbxoic.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gwuwxffak.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/guxqqgjjs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gytxhvrzm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/guerkrnfz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/grgpqbwar.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/guuvfuqpt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqhaabyoy.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ggjqnoytk.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gvjgqzano.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gcrgheuwx.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/glxmhggoi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gpmweigyc.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/ggdsfreha.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gzdadzjkq.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gllswusdb.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gqyklwdzk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/glofaybqn.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gbpqdlscd.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gppucknfr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/grostwdzs.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gvvcoytrv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/ghbysvhqg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gssvzkguq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/ghvkjhbqv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/glpewxjlu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gszfgygig.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gpfyfajlf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gzjaouokn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gctfplerk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/ghdqztrjj.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gqgccetqn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjyglsefh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gkvrgwcwb.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gmctvudpr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/guactcfkb.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/ghfisxaha.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gfanoeavg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gfffiqqll.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gendbawki.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/grvxlnvlu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gwmtustjq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gcyqwrlso.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gxqzfmhdw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gowhzhtoj.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gyokjcoqx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gbyttldux.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gtjohpfci.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gapjhfxax.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gyokrmiii.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gfxlzpbpx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/glwxtjbjp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gsfykjliz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gmuaqjwha.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gjdcrmmom.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gjjwfkkzb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gefkknugd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gmiaasewb.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gqfbwycme.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gdmbahyrj.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gwhdkqooz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gxicormaf.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/grarnnrhn.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gkyrlodji.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gskrezvva.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gmkmwelen.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gvxmefypo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gschjajid.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gjdgbpvsg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gnfutaeie.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gqbknirui.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gywzmpdzf.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/grfgpucdw.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/goolsfrvq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gaiynjalx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gxrjgpliz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gnnyzzgjp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gsbqyvxcj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gafaideza.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/goennnpls.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/ggwbuzmhc.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gcqzzzwpj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gbvsslaub.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gnxkwhziz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gxoudwpqs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/goortrmdl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gicyfikyj.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gigrkgxjb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gbflfevdr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gkomdkjlg.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gmxtyfevq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/giwprncot.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/glimhelqf.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gplihyjst.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gsctehybu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gsbtuuwot.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gvsaphwdy.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gdjlhegov.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gjxxhcowy.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gpvwkmfaw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/ghpjozlig.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/giprvofwa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gvjpxfdyo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gpjivlrcr.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gflmfmddu.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/ghxuivwlw.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gqkqjxqbx.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gfsucxpda.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gyvjbeeom.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/guwkaewwf.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gmqhgcqky.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gmzhqrzzf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/ghgboxrdc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gzgdmeyee.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/guyyhwgkl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gywbzxnng.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gbldlvyif.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gorvkecry.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gaszdrywu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/graczsopg.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gzigafffn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gvseqhugb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/ggmoprfcm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gopbteewo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gdymsbxji.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gxiatilzc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gebtiftqm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gtkzkhiii.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gymchbyzy.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gmiheeaol.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gjiqtazgp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gyvpdwdcb.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gqnsjqhqn.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gqtiizyos.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gldcjrqav.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gvxhtokbz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/geyyjvjri.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gdmqelkan.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gfcmdzsus.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gkbiarxgb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gukvvxtls.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gdudehwcz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gaovenran.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gqpeirtnb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gmkrfsota.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gytopaujc.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gspmpfvac.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gcqmpkyfx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gysfwgkov.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gntwtkkeh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gjyurafed.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gqoqtttmw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gypxbohvg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/guhdwmglw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gibkffrbm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gzeaxjiqe.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/giyzbjngw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/guzgsgchb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/grpycqmgn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gtcsvifih.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gnniygawl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gglzxjhdo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gggnojgze.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gbbjjphpm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/goyvqcqiv.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gqyquhgkq.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gucucpcxg.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gmcfbvzjz.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gcnyqczsx.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gszfeihxh.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gbpmcxwry.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggjdfokat.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gzkgmtops.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gfgcgfdjr.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gptqbkhhc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gvezwdxlo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/guqshamwb.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqrqggcdh.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gbaumcofi.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gjabtthrj.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gscbiblla.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ggmwdopgx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gvhszpchb.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/giyjqdgye.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/giccgtzwc.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/glowovdkd.sHtML


<!-- 参考信息 -->