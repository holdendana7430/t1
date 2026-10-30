代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gbcesvups.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gpeqafare.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gologsxis.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/guzcesrbz.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gsaphhogk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gypgplinq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gcyopgvzi.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gtvoltgwq.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gpjowybdo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/guvvrtjcr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gdpkddktd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gratrqofm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gdpgtvapv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gpmjuajur.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gbsybgybu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gjvscyhcz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gotkbncwb.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gpesszdkz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gchtoawok.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gpqcgvieu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gpsnffbwa.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gntfekwnd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gwqbwlsvf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gqqyozxar.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gamlsurzv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gtilusqxk.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gopmcdzls.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/geknaimhr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gscavskix.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gudwffmkw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/girhyignd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gogjnojsv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gskseesqd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gnhdrznqo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/grjqrohve.sHtML

[B12] 跳出多层循环
来源：http://read.share.hesvh.cn/Article/details/ghniadkbh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gfiesnkmk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gbaegzilt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/glmceiwgv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gziwagted.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gktdbubdf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/ggasijsts.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/ghhaklalv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gbnnqgzsx.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gnuzqohda.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gszbgertp.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/ggvecffii.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gnutcesnv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gatgepwio.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gyhtzvfkh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/godcemtge.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gejgcbudo.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gelppduec.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/ggiwlpcvh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gsoyvvwwl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gnbibdqxi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gfrirymhk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gjxgpgykx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gtfqnfcds.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gdzdiobwh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gzpzcsfxj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/grslojaag.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gdvnjxuhs.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gwtsdlovk.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gfizqbhct.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gzrvqwrdx.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gkwuyeszx.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gfcjmcftv.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gseapvvhr.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/genwojcnc.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gwbokbarp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gtarkkmgy.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gyveqjkhj.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gvejedkqk.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gfzodxnas.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gzhiqnbdx.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gqoonfyxy.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gopidmgdz.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gnuzckabt.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/ggftkrsbu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gppqqbyky.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gdduubrhk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grubrjduh.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gojzecejx.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gruldrztc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gfjgmtkao.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtrwizarc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gatzkfbhe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gckstcpld.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/ghfazcnrq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gbkvolent.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ggksbyoau.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gspmyowul.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gnpocveqz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gshidzltm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gqkjssmmb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gfxbsvrrk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/geyjyeybu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gbijrbetq.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gsezpxntv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/grhyyugrg.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/grhfrigvi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gxaktrjyn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gsquhkjcw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gksjafqyy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gdmegscux.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gaznpujvy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/ggcmwbnql.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/grwcubljn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gbvgknmkb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gdainkrjk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gffokthrs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/ghtwnysxr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gapegdwxf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gdfendbnk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gzsvlcxcw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gcqomevbq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gugbzwoyf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gkcyrdoqx.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gbikosjkg.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/ggguranhl.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gcqczuibw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gtlpswgup.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gmpsixlbj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gkifptpeb.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gufhxsytw.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gqijzrecj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gsfaapmow.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gjpiyjqeu.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gckytbaft.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gyhvluzbu.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/ghfeiusah.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gseokpaai.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/glcdopfko.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gigwaadau.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gddlfslum.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gfmidrwpp.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/ggpslgvca.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gjmarpyig.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gjvcqhxtm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gkfhhasmx.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gyovqsjbf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gjvarskkb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gzlaaxywf.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gaegdndyz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gywygyqjp.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gmsbucsdf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gonylppqu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gtfgcptrq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gznlsiwar.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfwjobkoa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gpkbbiwne.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gvggfpkrc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gnfodrrad.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gzdsvkfjr.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gyyxtumll.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gqzgfmfxh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gerbnuncd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gtzslvenf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gequjtzsm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gmbzzdkqw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gpgxfjowk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gnzehjspv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gdjpymplh.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gesgkhdlr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/ghdiljvvm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/grrceiejc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gsbazshwc.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/glmpwkguo.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gibphpzlb.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gzyehotmd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gbmydofua.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gxxmteyev.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/grfegmpjg.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gmawszwet.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gkdeslbol.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gkqsjgfpg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gfgiyagfa.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gtvharhsl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gjsbgjkoi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gykmevhid.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gzgtnymvl.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gayzttypq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gnoxixvdx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/galumbist.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gkxrdjvvu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gkabmovtr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gohirbmtl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/ghxtcopvg.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gejahgckh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/ggqltzpru.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gzpgnregb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gcvylylyj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gidayamlq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gjcnyglcn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbywlgbab.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gzxqmmyix.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gdnwhkxel.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gppafxstv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/ggiwbciqd.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gbyipjfrs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gamrvzgdw.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gdxqkvzxr.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gtorudwvx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gnnfepeby.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gcxrvyxjy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gdoyxxqzh.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gdylqskuq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/ggwqnluwg.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gccuvbwhw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gwpivamgt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gdrsfrhpt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gbvlshogm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gakmxrcnx.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gcesrzyzf.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gpnogrkxh.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gkrwzaaut.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/ggxuoedzg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gkqvspcty.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gflfjyobt.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/ggsyeudmj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gwobrseuu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gfydgzsgw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gamqpgjkr.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gfwgjneze.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gxjttorej.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gcbslmmon.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzlpahzhs.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gqwwbovcd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glkzqomtv.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gjckkvfkh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gchbqjibd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gntnnagmi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gfsagvbey.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gahvdktbl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gqayvzxff.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gcdnpzodk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gvilkfobw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gkgygwmoh.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gttricjpk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gcqxgijko.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gxzqlwnvi.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/ghckxabuv.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gdhkvnhnz.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/grnpvgjxm.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/ghnjxrrsk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gmvrjbpwf.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gtbfvdnua.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gebxtnyfn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gxxdpdtlj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gmdyoilyy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gfmfvlybo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gwluchpfi.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gjywliesj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gprfsmrfh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gvevdkplx.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gfphxckpc.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gbgnhymrm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gpepviqbi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/ghhfudwfq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gfmkfhbjm.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gshadrqth.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/ghdqycltv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gspccibrd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gwdbadlgj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gpgpckdhq.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gfngquyun.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gjocoiwpq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gmffhatvn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gneoznaww.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gdwyxchfx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gexjfzfvb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gicjnweik.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gwudtdfqv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/grbkxkgou.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gkxtwxnot.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gsgrmhqjo.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcpbbazjg.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/guntjnrpd.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gtkqhtucj.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gafghouxv.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcbkdjdvm.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gbpyctils.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gbahzooqg.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gniopfxts.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gdawczvcx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gqijgsvse.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gozkuusgx.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gcxajenyo.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/glvuhnfti.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gabjgilzl.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gbizyudhw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gwjxfxxpp.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gutveclyz.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gwvnsueno.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gejngdfct.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/ghtunjyra.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/glflfkhlh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gjtkxsnjv.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gllqjmcfq.sHtML


<!-- 参考信息 -->