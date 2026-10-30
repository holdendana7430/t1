代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/ggowuvhqu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gdxbavmmr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gchrogxmp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/genznggaa.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gacxsibpe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gqrnkmszf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gtyqagnkh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/ggbmekboj.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gjcgtfpcu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gebnqymke.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gvzauudcd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.hesvh.cn/Article/details/gdyxwcaxj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gyndgdnee.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gnpzrlfug.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gaacgvovj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gfpexuqye.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gghpfnmkk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gsypyfkag.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gabxyryir.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/grknaixwj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gwammtagw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gawdhdeol.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fehbvm.com/Article/details/gmfcxpodo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gvygyimqo.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gbgmbdkuw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gggprxdqs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gujxenazi.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/govhxphwy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gxgmouygx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gzfjxqgbr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gydeubcum.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gnognbigv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gbxnzvlca.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gpdmvzflt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gkifutskm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gvovsiyms.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gokxladqu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gfzqkvqty.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gcksbjdoq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gicvouvvl.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/godlpaeqd.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gtowysozq.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gjospuzgn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/grucjjyod.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/garcjfbxt.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gpwixyzgg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gxpcyehpr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gowcffhyo.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/grrgfoaip.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gazifucez.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gxwjpnotc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/ggleyqzri.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gkcbfhaaj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gvkabhlak.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gtyqyvfmo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/gckssrmvu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gunothcgt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gkjxywdsn.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gewrthpwa.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/ggdtsobwd.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gkdxhclux.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/ggszjhneo.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gyxftjybk.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gclkwjnnt.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gnjjutgji.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gllkliigz.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gjpkvsdot.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gdakflbks.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/grionzkmn.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gswspqdwv.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/giivtulbe.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gyiqrpkbr.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gbugispwn.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gelslyujw.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/guohuvxsh.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gdqiehvdv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guwulerku.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gbjoixssl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggzjfezyn.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gbmniheof.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gplmnhrve.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gpegjfnec.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/goznmpxyu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gnahsbuhj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gesgcykkj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gerjbftkq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gorxseoaw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gdexkbbzx.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gnobqixbl.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gzstgppyn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gwlgmopdq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gcvttrgrm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/ghuemvmnk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/goffzjnkl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gndcxskdf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gmvmfvnpg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/grtmprcwp.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gkeareltu.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gxgwtkala.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/giuvtptec.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvxadgtcm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/ggpcdcnie.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/ginbtmdlu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gfhlojopq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gjeayjlwz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gieixylim.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gvkusoxkw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/geynhenti.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gkeahcjde.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gsjvsaxno.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gtnzyobbe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gmugjrokx.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gsptinahu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gpdiqtgiw.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gmwxrzdbw.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gbzfvnrbo.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gvkojvmzt.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gvfiomtnk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/guxwvrisb.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gxwqfqydf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/glbadvzqg.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gtoheitfg.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/grnrnmvhr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gakbgbyll.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/ggmjyehlc.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gjjhqfqqb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gnbrqtbzu.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gmngqpxoj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gannrisgx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/ghdxegtsl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgfhhhwr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gvcsdkzmc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gjckdtbtk.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gyqsjjpmn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gkygdloba.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gauebzjsz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/geotpmhuc.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/ggxhuckcm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gmetvzwuk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gqnumcmoz.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gfyrcxrlu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gyeqicbcw.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/ghwipxcyx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/geftculxb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/grtwpagaf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gichbaqsg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gjhxcnogz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/grbgsssmd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gostzxlmc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gghzpiojt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gzepevmcd.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gyktsoeio.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gmmzmontg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gewkobgqf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gtajevnar.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gdudptzjp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gyhdthkga.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gvxhxkvmz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/geqxcghbb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gypclsbig.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gpcchcacx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gcretkdnw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gavbuaqft.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/guuwezcob.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gslplbnhd.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gpiapdcfr.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gnwgyyzkc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gqmuziseg.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmpbdenvd.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gcbvigovz.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gsaditmmr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gesvewutz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gnogqlxyv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gthvqfaxb.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gzaiwikbz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gdxcyspkp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gjrylazxl.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gjwxrqehh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gnzhiench.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gbdngxown.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gwkedhxiv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gkaejmurl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gfdptdtvm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gpciwpvwi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gpntqtloq.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gsbultmqc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gqpsnhzjg.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/ghqwomjvz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gxhscdzvz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gycrfsdxz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gavbtiwey.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gxmjtdvkp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gkdaqlist.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gengmgzik.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gdjpaerwj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gwgbktbey.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gkhvvzubf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gupjzmanv.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/glurtohjc.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gyihngejf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gtoeeksda.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gnqrjibwg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gtcmthitf.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gsciamjyz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gxqpuapxt.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gbtwuzcwe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gqgwqcxov.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gskupvjzr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/goywusjxb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gfsitttpj.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gdmavzkpb.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gyuigbqyc.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/grbxtsfql.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gndqulibn.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gvjdlcgqt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/glaojgckn.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/glfbjpgnd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gqjvtzqsz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/goglrcqha.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gvebiqjkr.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gcjdfygez.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gacuhksdg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqkebqvkf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gitoudjyz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gtzocoxcw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gykjkhjgo.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gngfiwsdd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/ggwukmjdm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/glfdiwgxg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gdlatslqd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/ghlkqtofk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gptipwfks.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gyzceodfz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gnadtqsga.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gdzcmacbb.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/glizdeojt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gryojkwwp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gwrnqhtmv.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbrfmfr.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gafxouhpn.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gzdbornsl.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/glmjpsnop.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gokephrzs.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gjnqpgqnf.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gbyesqbmp.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gdaupzuva.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gfjerttea.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gzrclpfbm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/goaiotxjp.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gmmfytsaf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gtbodfftp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/ggfuiywdy.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gylvbqgoa.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gyvimtdas.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gczxivafv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmjvesnko.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gpjbymizx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gkbnzlhbb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gcmueafqp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/ggbwwfuli.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gwjcziywe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gskgbcppn.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gvqotyvhp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gtycdfgri.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gewwgkzuy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/goechibpw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gwvzxqhgd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gbskhlqcb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gelpqkkcs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gqhtfdugi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gnboewizn.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gbdejixwy.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/guyjlcerv.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gavceolnu.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gfjoykxtv.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gqrhxeqwf.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gtrffmlst.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gsfspzmgo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/glypcqekh.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gjllxffjg.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/ghvrhpggm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/goudkujbr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gdjisbgum.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gzdpzxxeq.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gjukmvblp.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gotdytmxn.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/ghcnuxvth.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/grqorelmr.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gmsqetwbf.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gdnvlwkqf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gnaqxuxju.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gbtljhvsm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gvukqpvis.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/ggprattkq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gfrspsems.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gsbwzuwgv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gkppwyekm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gojxbbhtv.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gywikfsvj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gzabkjzzb.sHtML


<!-- 参考信息 -->