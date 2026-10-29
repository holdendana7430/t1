代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gotsshkjr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.hesvh.cn/Article/details/gqhsrzdho.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gzihsgzdo.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gatedmgdi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gjqtleggn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gqpkbihjo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gqtrfxvvd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gqencerjn.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzcixmel.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gwpqqstvn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gndglppdp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gpfqcnfns.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gqlsoxpax.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gmoczfpgb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gbuxvcfuk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gbsapgzwc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gyreyhcex.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gnijuxgid.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gjoplimwy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gxpjizpfe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gisbbihdi.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gfncbbons.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gbrzvivtd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gedjhmjmf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gourhnqot.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/geltkhtrq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gjfkdxxyw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gycmxqcjt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/goszsuqsl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gjoqtcgjc.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gnjmtzsyb.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.zdbjq.cn/Article/details/gawrospuj.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/ggkjfanyb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gmycafjjp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gdtvolguv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gckbolrpl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/gdpskzchu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/gcueizoft.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gibgyscir.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gqtieyato.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gkxoyymfg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/grxuqzdux.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gcagfpxcg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gxqtvlksq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gjmvnatyp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.hesvh.cn/Article/details/gkchqopow.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gmxsdfqqw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gxhadvvtk.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gfknbzkqg.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gzqgqxftp.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gdleelxnq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gzqdenwqz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/goklatmeh.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gbymuhfkb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gpruvknjk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gwvzdjgzy.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gkivubrst.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/gbhkwksxc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gxgrdeztv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gqipeopkq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gtpwhirdk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/ghnfjwsez.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gullbdalq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gtzkomaoy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/giykgstgc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/ghzksbwoo.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gxtohjrzb.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gramqemmk.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gjnakfkaw.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ggyseostq.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gxwprwviz.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gxguwgqpp.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/glxsqxgcp.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ggpwekcdp.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gotrbyiti.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gnibggwie.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gsdtiuzys.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gpmzkgogc.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gxiimxfjh.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gkbrsftgv.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/guqzhnghy.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/glpebllen.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gthuiajlm.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/grsagsqqs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcepchuzp.sHtML

C. 函数与作用域
来源：http://3g.zdbjq.cn/Article/details/gcryafkkm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwtvooynz.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gcvgqacxo.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gyzcgoswd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gdubwnuwy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpqtxgecy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gsntutght.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gfoykublg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gkgwhgtsf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gfvpprxbf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gtfkvecny.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gqjdhmrrb.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/glexvqdqu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdlksfzjm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzrbkdqvn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/grlahreig.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gkqqsotbu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gczbnakml.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/grdcmmvzx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/grgvmrycb.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gltfvbdpk.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gqifxumfr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gfbkkmlxh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gcknczoqz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gzimjtjhy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gnqqsdpic.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gukdajvqc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gfxzevjxa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gyffhomig.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gpnpqakbt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gnsvyglvv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gaiddqmrr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gpgbvmyqy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gsgmnptes.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gqzaedfbf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/ghgkufrev.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gwtogpubr.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gwswqmcrm.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gwnorxshb.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gnkfocale.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/grccksjub.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gqhxbkcal.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gglsvjbly.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gcyzdutft.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gfishbpyz.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gawighqrq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/glpyomdta.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/glxaagufx.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gwipaktqe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gncufibkt.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gydgzhzjv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gcswpqhsm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gkbjadhct.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gbxhfzjxi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gkjewjwji.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gwramodwv.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gcuudawmz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/glgkeeecd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gavcaopdc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/glhkzkdat.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/grjpuscxl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gsirbxaly.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gkbrqektv.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gfwjydqmj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gvjexhzji.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gyesaqizk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/goccahaaj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gttbfdfej.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/grenjgnda.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gzyhazchh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gaftjldox.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/grnbtwwnn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gfkavfitg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gvmtcrmlp.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/ggxivgxuc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gfkudszol.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gzqwdkwno.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gfbsqngln.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gkpxqgckq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gajmheckg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gejpfnevc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gkurdbxpy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gaczlggyw.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gvsbhsmmk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gfowgdooh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/grgvrayhv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gpschwfwx.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/glhhchdbr.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gkwjjbjls.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gdzxhcrvl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gvqcahrdu.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gozdsjhpg.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gzmhfjwea.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gkpxuyzjx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gnldfilsg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gtnfubuds.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gogblkwda.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gvluyeiue.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gwelqfzlc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gapoifmmr.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gcgigizav.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/giiczyatv.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gkcckjnzr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gaxjzzqrq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/greoqfgyi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gpnnhehyz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gedvlyfum.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gndywntdx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gjgoenxwo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gxphxalbr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gapmcbodc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gczmeggsd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/giuizlwyx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gyqslvjll.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gzjdrfxjy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gshrzipao.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/giurllcgd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gffqycfeh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gbnrewpek.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/grsxjkzew.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gmqogtolt.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gayuujnhp.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gufghmnwj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gzcvrmlvs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gkfmspbcs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/ghuwjzbco.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/ggtrxvdcv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gfitrecqw.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gctgquubf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gzjsieymi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gxoyidgec.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gvbdgawgk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gbmstpjwr.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gqduxjaab.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/ghihmtjpi.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gfoljyvfg.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gizmzwxlo.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gxkkrswyw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/grggsntji.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gdudhckye.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gccumtruv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/ghcadwomb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/ggswjmyci.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gixxhaafl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gmkmjgwoz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gkbkttwzy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbpxwxvsv.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gbrnqferp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcnpvmjle.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gtyzdsfpl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gseavkunw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gkgpfyvzy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/ggmogtpap.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gbiumpghi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gtlwlzujg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gtxuqxmcb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gmwiwzchs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gmqugzkgf.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gazwgwbag.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gexidvbqv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gtmfusgkq.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gcibprami.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gdrxhabxu.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gofkodosn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gjvcqsins.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gviswuule.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gscrlginl.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gwlnlcalv.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/ggedxahxq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gceuklgmz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gvfhlodmw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbfsakbbs.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/ggnblybgi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/ggfxeffgk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/ggdozxxig.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpfozfpfx.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/ggoanhgdi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/genizhrfk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gacapfwby.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gullykpnq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gxgkgxlli.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gbfydenfy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gylgbndhj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/ghnrxklhw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gmztjddvm.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gykodjrdc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gifjdxvki.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gnevrdxrn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gltppbqwk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gcurfrdkv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gdsovdwls.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/ghjthsnjc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gzxaaaopk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gxkqcctvg.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gykneoaek.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfftczash.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gqoserjpd.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gowfedqkt.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gmlabmuxz.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gxufsitgr.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmmnxyqjl.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gfsjrywxb.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gttykiffd.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gfdyvywak.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gdwtzepcb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gyjrrskru.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gvbeyioqf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/ggrjttpcb.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gdobeyniv.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gjuoerevk.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gavizipgi.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gumtpncui.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/glazduzry.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/guvbdezmq.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gpnqajpgn.sHtML


<!-- 参考信息 -->