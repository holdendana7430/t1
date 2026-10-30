代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fanxiaobao.xyz/Article/details/gesuwjmah.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdrqwshy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgncobli.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhztbqjf.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsdbxoqm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmfiqlpl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpsktljo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmnnmxut.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqacwcbq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fanxiaobao.xyz/Article/details/gbxhfffqs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjphsrdlr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzauzoitn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/grcoxwemc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmhtrtvn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxequyouh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/grzvyqfun.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/grievuhbu.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdemevkff.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fanxiaobao.xyz/Article/details/gjenuaoki.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsgprkllk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjdfmizv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/guzbdwoeu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fanxiaobao.xyz/Article/details/gndrtbudb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzzgdcsg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fanxiaobao.xyz/Article/details/guqlyjgfe.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gzpdfcotg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljoebbyg.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsruyevyg.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjqbcwqm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcesimvha.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfawrpwpg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfkhfznt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fanxiaobao.xyz/Article/details/gmlghshjz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gdftgiyed.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gbsqsnbcm.sHtML

[B12] 跳出多层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gtycehgrk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhnwdxfb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gnrlmtlix.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbxbraz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gjnygqhnp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrbayyrw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwedvijqd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fanxiaobao.xyz/Article/details/gzesbnjgq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fanxiaobao.xyz/Article/details/guubkqhdl.sHtML

[B13] 判断是否为数字
来源：http://baike.fanxiaobao.xyz/Article/details/gswstickt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsedcwkz.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvboypaou.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnrmlorx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqduzylyn.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtoibkcg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fanxiaobao.xyz/Article/details/grhxjnnxq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fanxiaobao.xyz/Article/details/giqmnjnig.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fanxiaobao.xyz/Article/details/gyosnlmmz.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fanxiaobao.xyz/Article/details/gdmozxkop.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fanxiaobao.xyz/Article/details/gbzdbymdd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fanxiaobao.xyz/Article/details/gdmnvvfll.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/geaehmwjy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoblesie.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/ghhdnsbcs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geicqhdiv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ggxitnfps.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzuvxhwp.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/gvypvaspg.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/gthhvrqhx.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fanxiaobao.xyz/Article/details/gslejmuyw.sHtML

JS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/grtgxinpd.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gawdboxrp.sHtML

Java: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gtntjaizf.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gnqfgswos.sHtML

Ruby: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqvchbuz.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxjjiijs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/grwqxyboe.sHtML

Py:   if not data: return
来源：http://m.share.fanxiaobao.xyz/Article/details/gowomtsmo.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcbuotxj.sHtML

JS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gaumxbxln.sHtML

TS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfendunjk.sHtML

Java: if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gymjqjgwz.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gvmpboqbh.sHtML

Ruby: return if data.nil?
来源：http://read.share.fanxiaobao.xyz/Article/details/goxctbvnr.sHtML

C#:   if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gpoqvotkb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gacydtmjl.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gickigvuh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glnfjkdbq.sHtML

[C01] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/goxgmjmsw.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/glymqvguq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuhchtbh.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhzemeia.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxceahicl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gywsvhvgt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gsnpmyqgh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gavnsdrsl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwsjwjjpx.sHtML

[C02] 默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/ghegxfyvz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gafrtdnvc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghetmjbhi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaymgeaq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegasytbt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkxqchqi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhxskwfb.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbrptnib.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdendnte.sHtML

[C03] 可变参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfarxyljd.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fanxiaobao.xyz/Article/details/glhlyuzif.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxxpraxb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiupeagq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbzsmaqs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gkgcbnyhg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fanxiaobao.xyz/Article/details/gzsnqdson.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzicubhbv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhcceyix.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gutczygck.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fanxiaobao.xyz/Article/details/gkcvklhww.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdciwipp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdzzzwcq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhdozaef.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fanxiaobao.xyz/Article/details/gkneezcfn.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gatfzarcw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyawpafzi.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmeawwed.sHtML

[C05] 返回多个值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpjlfxaf.sHtML

Py:   return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gfzczwvlx.sHtML

PHP:  return [$a, $b];
来源：http://3g.fanxiaobao.xyz/Article/details/gjocyujym.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhfcewgb.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpxxqcuu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrqknioi.sHtML

Go:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhsptiyg.sHtML

Ruby: return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gpryhbifi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbgtjygq.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfrkkkn.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fanxiaobao.xyz/Article/details/gbdwgkknv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gmqgkrzvd.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjpbwucn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfddwfprd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/ghooxclga.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyovnlxo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/garojfhhh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaagzgst.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fanxiaobao.xyz/Article/details/gemcztulq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/gutqecvas.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjusjnjos.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqmcnwdg.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbafmazk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/glwzucghj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fanxiaobao.xyz/Article/details/gczpuyojh.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfeorlrco.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfutxjxi.sHtML

[C08] 闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwjrmckq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fanxiaobao.xyz/Article/details/gqekuoyjb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmgufxxo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtgctbnks.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/geigwxudv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/gnccqmywf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fanxiaobao.xyz/Article/details/gzteqmmjo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqukdwan.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grudweydh.sHtML

[C09] 递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgzjcjlb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gaqhfshwg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbnrujlym.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gtynccnmy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gelsozvds.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gzvbsjgls.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fanxiaobao.xyz/Article/details/gyvhuqqik.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbkpiawa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvivacev.sHtML

[C10] 变量作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgogvpkg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlkhmdcb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fanxiaobao.xyz/Article/details/geatsyext.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjdqbocg.sHtML

TS:   同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjmxueft.sHtML

Java: 方法内为块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gjrqxkqmr.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnhazbse.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwabbtfv.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrhgevyd.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnxihmac.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjyhldfc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fanxiaobao.xyz/Article/details/grhjpctbz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gaipihzsi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fanxiaobao.xyz/Article/details/gzjiyjjxs.sHtML

Java: import java.util.List;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggysnadkx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuonpsiy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/ggtpsqlwk.sHtML

C#:   using System.Text;
来源：http://baike.fanxiaobao.xyz/Article/details/gbmzvypam.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/ghnpzqigg.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fanxiaobao.xyz/Article/details/gtdklqxoc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxpyqnju.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gpozgrrvx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeuaayns.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fanxiaobao.xyz/Article/details/gotqassfk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/gucngrvjp.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fanxiaobao.xyz/Article/details/gvhwrrnst.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoxqakdk.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gokxbpskw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrosasxq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/grepexdjn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfvijvjy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghowifvjb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedpfiszk.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/grcpnjxje.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fanxiaobao.xyz/Article/details/gpfldjces.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhceojes.sHtML

[C14] 泛型函数
来源：http://m.share.fanxiaobao.xyz/Article/details/guvxlygmr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhxhxuob.sHtML

PHP:  // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/grewvsppp.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gzmygkvbg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglaqefxx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpdtpgkzs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fanxiaobao.xyz/Article/details/ghghelias.sHtML

Ruby: # 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/goqdzbcwg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fanxiaobao.xyz/Article/details/gskhtmddl.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gycekyurt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fanxiaobao.xyz/Article/details/gupowefxy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcycbwkdl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gyqhznkap.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuihjluq.sHtML

Java: // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnvhipno.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcbnxmnr.sHtML

Ruby: a, b = pair
来源：http://blog.fanxiaobao.xyz/Article/details/gsliyjwur.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqapxeqp.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvthtufz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmkbkaaq.sHtML

PHP:  // 无重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqgojjnd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkmuvxjq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/gcxllqpmr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwxwqubl.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/gakknkwks.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fanxiaobao.xyz/Article/details/gusfbhyel.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbrojkary.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdewemcma.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fanxiaobao.xyz/Article/details/gnynyrrcj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhoebvse.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gddyjsydf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fanxiaobao.xyz/Article/details/gikvhhwtd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeoblxom.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavxkvwfs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gbvxihgvl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/gbjotqgyp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzgicxwt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/giwqbmspa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fanxiaobao.xyz/Article/details/gsfrllrae.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnldzqkw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fanxiaobao.xyz/Article/details/gndngwsyg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzdgruyq.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gmebpuqji.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gxlvjpbgs.sHtML

Java: list.add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grasijyrp.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfittpelp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gowvbidro.sHtML

C#:   list.Add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdzpuwuk.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdclhravf.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqcosulq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gosbenfcg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fanxiaobao.xyz/Article/details/gowykyffc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbmcvhrs.sHtML

Java: list.add(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gwzwzjzyb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmnyvwzp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fanxiaobao.xyz/Article/details/gqgqrzsbh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxaobfgj.sHtML

[D04] 删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gomjcbqmk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwewjiaaj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gvgevrkcu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakeqjiyr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxprrmwil.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gabcremkz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaitbjra.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwswwiqrc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/guuosrrgu.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsryjsaju.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gbigsspaa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfpnztrl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gxuzwyaqx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzoancxm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fanxiaobao.xyz/Article/details/gimgnxcaq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gfabbwkpr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfsesbmk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqblvdej.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gadldsmqq.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsvcasey.sHtML

PHP:  count($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvxrgueq.sHtML

JS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gurhivptc.sHtML

TS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdgernpd.sHtML

Java: list.size();
来源：http://3g.fanxiaobao.xyz/Article/details/gfcrzolln.sHtML

Go:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhplstsj.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzabsluox.sHtML

C#:   list.Count;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbjbwnkl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidmkcnbx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/gvobyauqt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gokxtczqb.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gezeczymh.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyyvcqej.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gbdspfcta.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/gtmikfffq.sHtML

Ruby: arr[1, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/gghicdyig.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/grahsevkb.sHtML

[D08] 合并两个数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gcijmdcik.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhejvkdv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorkoxxnv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsmdapzq.sHtML

TS:   [...a, ...b];
来源：http://mobile.fanxiaobao.xyz/Article/details/ggywqwgmc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/girgczucq.sHtML

Go:   append(a, b...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhnoigsa.sHtML


<!-- 参考信息 -->