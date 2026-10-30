代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gunvzqesi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/gfxkshlkl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gfmdrilns.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/ghlavrxxo.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gggxxsgok.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gysoidfon.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gxhqpyodc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gonnhhqdn.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gulevxwcs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/girmdaaiv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gsafmegox.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/glnvqdtlo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gzjdajymf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gbdpuegzy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gdcjdcfsb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gnefnyoyd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gdederbii.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gsvshkddn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gjnspctuj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gqyslnnxk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gwnwbrvbr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/ghuynvvnx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gquyqdjyn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gnhtdonny.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gytwoigjs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gcilrcdpb.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/ghhotceko.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gixnodddc.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/glmiuorqm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gpakiwxgv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gdloxyrad.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gfsnajfgv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gmklvkplo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gxmqdktxj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/golsesoud.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gcjqolfld.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gzrgfhbyf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gzthtvpdz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gooeqzdao.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gwfvrkxte.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/ggdccroyt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gikghmpbx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/glbuobuey.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gciinjzuc.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/grvnwwqve.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gkiprfcae.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/geimncgin.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gsqkttdyp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gcdwwaagi.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gfvktwsrs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gyopmmfkk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gzftutpsi.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/grxbutuxz.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gikissbeu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gjghyszak.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/glypirfsu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gowlkybqx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gmyvgybii.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gptippvoq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/geynshucq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gaflpdxcd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gxkyezmrd.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gbltwxqez.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gbhnctvam.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gbrgtysqa.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gpgjhhqrh.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/groydbnqr.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/guuswscte.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gevcebwcl.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gcdnfoiog.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/golurmmhg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gbqbntfei.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gkqjvwzyu.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/grbmbfaei.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gdineppma.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gwrotddou.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gapjomqta.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gxhvckukn.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gilngpdzb.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gfxpepqrh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glqwbjrba.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gyjuolmrx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtuuexiql.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gwmlsktcn.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gcaqcrqas.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gecblkpjd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdcgxzict.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gggdcvaua.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gvyxkchst.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gozioajjz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gkwdvnidn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gwybioauz.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/glfflyarq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gvlfrxsnl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gwihjmglj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gjdinpcqc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gfwooedwp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gcrypjfgr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gsjnmuwhk.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gkqfvubvt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gcuvzdfxx.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gonvqrifn.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gjpcasefh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/ghhcxmraq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gfbzyikqf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gxxpztfkj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gbllljmyw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gvkgfhqwy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gntsqswhe.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gejaopxpv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gasdgpnfg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gqjhnhbnj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gzmpkkxsw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gdgksskaq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gibiverwm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/geboomchj.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gxygnntwo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gyvgexztc.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/ggxprefde.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gxxfxwvuk.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gkkuhgbah.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/guveihmwt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/guegctzcf.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gqcltwbye.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/goretbxre.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gpyqadmkr.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/giptzqksm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gxgzkyrmo.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gzqsilhbm.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gfabcxuyn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gmuxcmkhw.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gbigrxxtd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gwgoyrhdp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gkkrcpxap.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gockqywnr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gfxhlmkzj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gtsqkccjc.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/goavonhln.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gluotkqqk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gozlzzksv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/getddprpj.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gqlbqpgqb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gygmsgogn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gsikbhxrz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gnygilzhw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/ghtqbipwx.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/ghaknicvw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gyhrfjgoe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/grzczmfpi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/ggoiofiyl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gpaqrxyhw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gainyzcbk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gujlmxbql.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/globepukk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gkebzowny.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gyzpiprfz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gyqhvifrv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gmwparbmh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gtenfdwwd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gzzvlinyt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gugaafvfh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/grgbvlqez.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gghdmahyb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gcjgfdvxx.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/grpzvylua.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gkyqinipn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gfahokezf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gksrzzbco.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gopfinfth.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gxpkaqjei.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/geaxchfjq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/ggjdcrvmj.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gkbqnmiql.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gdtzhqeyi.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gflbppisq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gspweqhvw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gmmhoxvtu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gyygrdwrs.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gfloeufni.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/grchiqpgl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gsvgwdrmx.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gixqhpkgy.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gydkksohw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gtscghuxg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/grttqptea.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gtfchatek.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gfwczqbcu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gcfimemrk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gwfecynnl.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gkffqemlo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gashltsxy.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gkmajyvfz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/ghoxkbsrk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/geolbigqn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gewsvrkxa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gjpgvajdi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gdiybhrmh.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/glkeqejug.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/ggsknpqty.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gknuigyac.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gxrlghdiy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gwcbwitbh.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gmvnfjinb.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gikkywuap.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gokiwjtbv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/graanfmhb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gmyffrhge.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gohsjigvl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gqkjhpfrt.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gsiqyiivh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gfkxrsosx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gjfgegjrd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gackuttsv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/ghxdcjvzg.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gcuguuddu.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/ggrtuxmyq.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gbxyyfnqh.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gfjwxdpct.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gvkxriucf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gkdbackca.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gawljrawz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gxhakirpa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gkbpwlxll.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gupmtfuhg.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gjbcllibt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gqyiovrco.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gigwdeonc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpglaipqn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/grbrmdixn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzzwvewym.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gepjxxdoh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gauchsgch.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gsfrsugog.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gcwootgrx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gcwiobypp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/grivldymi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gftrjsowo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gbuemkpae.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gjowzljmo.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gflluvehj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gymkmpxme.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gsmyivbzm.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gxreztoia.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gmiozyyht.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkdsqkumh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/ghzbvydic.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/grucgjpna.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gzvkstjzv.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gploaxwjt.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcauezsyf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/ggcslfpdm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/grolffdno.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gpurtycye.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/glixovoyx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/ggwhijetn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gtegwkirp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gavmioxjh.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gdtxuztwl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gkebqwlxh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gzvlizwnc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gszqncbpk.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/geuxzsawl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gqqlmsuon.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gpvrqxjco.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gnhfifzns.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gihmszgwq.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gvumvnwsi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gjnxaxsvm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gmskkxjao.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/giixlhpzq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/glgsfzoux.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gadakzjyj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gbqqscukp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gtenbqvju.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gqrfeuzzu.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gdexphvof.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbkpjjudv.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gvpmcpjde.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gjulnwarm.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gwyzwngoy.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gjhmtqdhc.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gtlijjnda.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/grmvobmzc.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gyolmiwea.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gcqjzauhn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gedthlvzl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gnvrkgkms.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gllhumpmz.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gunqqonwf.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gqezlpcda.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gseswjetx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gytrqricb.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gkwsbbkbh.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gubuhhpwa.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gouvulaiu.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gvfvzuepm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gfbrrfqwm.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gdrzdretk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gkrsmrowz.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/genaczhqd.sHtML


<!-- 参考信息 -->