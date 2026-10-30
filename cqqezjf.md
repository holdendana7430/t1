代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fanxiaobao.xyz/Article/details/gemxdffhl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtoqbyqdv.sHtML

[B07] while 循环
来源：http://wap.fanxiaobao.xyz/Article/details/gumehfgdb.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glflzgube.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gineucqem.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfahhecuw.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glhbkkori.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzteoktga.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfevkufrm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fanxiaobao.xyz/Article/details/gvqjztgmw.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfvrhacwf.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gratwtihy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fanxiaobao.xyz/Article/details/gxoembylo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkmdkcff.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqxvwmcv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gosuanmsp.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtieualnc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gyujgsnbw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gktkhtyxb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/glnhkojzr.sHtML

[B09] break 与 continue
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipfgwivp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwszqved.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzzxegij.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcgqmcfod.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmpropslm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjtgbgjru.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gmznyvolf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gegqdcxzr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/givixuztn.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqagfztwk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlxuxezb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwkejdhr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gsszqetjj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/ghunodhzt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghgtgmwyr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gbgtsyjai.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpdyaxjy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grxwdrijn.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fanxiaobao.xyz/Article/details/glezqmbhq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwynciug.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gzfcdcfhv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpthcadf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gtfpbshcz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/glnypedaj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgraorvk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzlybjcs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoutozfg.sHtML

[B12] 跳出多层循环
来源：http://3g.fanxiaobao.xyz/Article/details/goxfghjau.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fanxiaobao.xyz/Article/details/gqbyvhibi.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fanxiaobao.xyz/Article/details/gwpemnfpl.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcidavyvj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdldalaks.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gefxtmqze.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsnndbnm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgwrwqfs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gtlplylis.sHtML

[B13] 判断是否为数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gikdsrjdj.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fanxiaobao.xyz/Article/details/gdjdwooyz.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmypqsae.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxrawquu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gfpjusnbj.sHtML

Java: x instanceof Number
来源：http://www.share.fanxiaobao.xyz/Article/details/grpvvxyra.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fanxiaobao.xyz/Article/details/gwmcqaluo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkbtbczk.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpooldzp.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/gwralijqf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fanxiaobao.xyz/Article/details/gpoftmqzm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkygsckor.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gcdazbyrs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gosjbuhse.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbwteugr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdrrsvtj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfbkikdv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gjazvqgex.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fanxiaobao.xyz/Article/details/gdputofyw.sHtML

Py:   a and b or not c
来源：http://baike.fanxiaobao.xyz/Article/details/gznclcxsx.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqmjduba.sHtML

JS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gohxpwnie.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnovqgruu.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmfdihwi.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghyehjav.sHtML

Ruby: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gbsrynlku.sHtML

C#:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gzilvpyno.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gibisvjjx.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjqueckl.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fanxiaobao.xyz/Article/details/gugdjsiqb.sHtML

JS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gldrmsanj.sHtML

TS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkzstgeb.sHtML

Java: if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/guiprbfqq.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxbiueoy.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gponpjpdu.sHtML

C#:   if (data == null) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/grzxzefgu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/geeyqvajf.sHtML

C. 函数与作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxhtcnrd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gesccmyxe.sHtML

[C01] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gjabilfpp.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gipscxkat.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkgsaudu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwtlxtpd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gunanjndk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvaxftxh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbktcvxe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/gjdkwsmha.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/goignggck.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwutvqeom.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdtuwjyi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsdvoldov.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gakulukpl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdeqyknsm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gccrfyfpe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fanxiaobao.xyz/Article/details/guepeeflm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiryqmiy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fanxiaobao.xyz/Article/details/gzharcqka.sHtML

[C03] 可变参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrukpwvt.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghadczhhn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghauzsqgo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfrwhdmg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjnbotskk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gishmovck.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/gzufnkwnj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gfhyyhtti.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fanxiaobao.xyz/Article/details/gnfxjoqte.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgauvwsf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fanxiaobao.xyz/Article/details/gztqozgab.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwrxfcdvc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmaxbqpmz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gplfnsulg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givsjttli.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqstuxdn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmlpmaph.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiejpdxt.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjstgocrj.sHtML

Py:   return a, b
来源：http://blog.fanxiaobao.xyz/Article/details/ggtdgjmkb.sHtML

PHP:  return [$a, $b];
来源：http://3g.fanxiaobao.xyz/Article/details/gpszckooh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoydesnw.sHtML

TS:   return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqztlkqv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fanxiaobao.xyz/Article/details/genomhdei.sHtML

Go:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpjadiug.sHtML

Ruby: return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/girzluacx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/gsjcvfjbq.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gopnyyjnh.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fanxiaobao.xyz/Article/details/gjdxpssac.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjvwiiou.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxyxpads.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gylwhfwmr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfsuvpfo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxgjydqb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gndwhgnjc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsswdhzvh.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fanxiaobao.xyz/Article/details/giigmwgvq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpumrakw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouorwajd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fanxiaobao.xyz/Article/details/gihpodxsq.sHtML

TS:   arr.map(String)
来源：http://wap.fanxiaobao.xyz/Article/details/glxhlibfb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gdoxpsgni.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fanxiaobao.xyz/Article/details/gyuohxrqt.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gcipfnmyd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuzofqfs.sHtML

[C08] 闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghnbplxk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fanxiaobao.xyz/Article/details/gfhsknsdd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggqbcukzi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdigjzlel.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwzyojhc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/glxbyoesc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyszobilf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fanxiaobao.xyz/Article/details/godntirjf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzvhrchwl.sHtML

[C09] 递归
来源：http://baike.fanxiaobao.xyz/Article/details/geikaihwf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwowsjnmx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggtvjephs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fanxiaobao.xyz/Article/details/ghfxbaltr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gzadvpbzp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/groxaabxe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fanxiaobao.xyz/Article/details/grpymczwn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxvvkslw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqsvpnop.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/ghnkbxwkk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fanxiaobao.xyz/Article/details/glherbqhx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fanxiaobao.xyz/Article/details/gpazfrpah.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gkmcxzkqh.sHtML

TS:   同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gafuuzthk.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoqqynat.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gmxhnlrjj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fanxiaobao.xyz/Article/details/gojenuows.sHtML

C#:   块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gezbjznwb.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozbcuctl.sHtML

Py:   from module import func
来源：http://wap.fanxiaobao.xyz/Article/details/guxfwqodk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhcjqezy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/goqphnrel.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fanxiaobao.xyz/Article/details/gywbezipm.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgfxpscq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrovuquu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fanxiaobao.xyz/Article/details/gftuwcchy.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcedloyh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstenhpvd.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/gubqpifak.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fanxiaobao.xyz/Article/details/ghrnkvspd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gwaupxymu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhaamccn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjegiujfy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxygfgxe.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/gmoppohhn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gykxkzsvw.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fanxiaobao.xyz/Article/details/gjgrwpuno.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/giluavurz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdxuuxmvg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fanxiaobao.xyz/Article/details/gkpiwmkzx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqvkzjqa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyruptwnj.sHtML

Go:   func add(a, b int) int
来源：http://blog.fanxiaobao.xyz/Article/details/gqtrqjcpl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fanxiaobao.xyz/Article/details/gyhduujqj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvwesbbz.sHtML

[C14] 泛型函数
来源：http://baike.fanxiaobao.xyz/Article/details/grwrnovxw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/gfsojdrlx.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvciatxw.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhrkxpbm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvggnokhe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxzdguhuo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmgiciiu.sHtML

Ruby: # 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeunckwe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjwnfmxv.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxexoxsg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdbykoyl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gakdineqv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glpoydcdn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gikuzjwqi.sHtML

Java: // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/grnslmkrs.sHtML

Go:   // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtxnjwzt.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdujyzxki.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fanxiaobao.xyz/Article/details/geujzinby.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fanxiaobao.xyz/Article/details/gtywfhxrw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglfhpevt.sHtML

PHP:  // 无重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/geymggdmu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gtxvcpshy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/guutefeef.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqtfufty.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsaatlyv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsvouefk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjklmmmsz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqtquyxb.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrclhhrb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpntwpdwh.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/goffuqulv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxpshscu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gdmojywvv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/goxchahzh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gitnkdlsk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fanxiaobao.xyz/Article/details/gbjzcvocy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fanxiaobao.xyz/Article/details/gadaukmdh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpvjvgcv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgswozvp.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhqomugu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fanxiaobao.xyz/Article/details/gllizfhmx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gbvkqaldp.sHtML

JS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrbbyqgj.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gsnwxpzex.sHtML

Java: list.add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/goddyauot.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqhmojly.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fanxiaobao.xyz/Article/details/gzczwiqfb.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gunqajpxl.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdcoxgxo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqxenrzj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/genohurdo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwuzuzny.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gchawtopl.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzzwdggr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fanxiaobao.xyz/Article/details/gxbtmfxog.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwmctoko.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/grrrufwii.sHtML

[D04] 删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzwphxbap.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gehmbixee.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmtcqkgr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/gomeejroe.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gcxcenczl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxuichoe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrugizkd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmypkhqn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsloxcifd.sHtML

[D05] 访问与修改元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gutkbgzci.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmbzdqrt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gttxnznqt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gdhqkcutf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fanxiaobao.xyz/Article/details/gieibkick.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gffgmwzgq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gkutoxgrp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gmsqkgyce.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gaeguuden.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnvfwenfv.sHtML

Py:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/grlfbjutg.sHtML

PHP:  count($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpybqtrzm.sHtML

JS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqcyuwha.sHtML

TS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gzknadelu.sHtML

Java: list.size();
来源：http://read.share.fanxiaobao.xyz/Article/details/gyluzbnqy.sHtML

Go:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gxakhqpgc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/gsuzahpqu.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxltgpauq.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gnidlsvtm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcycmadbo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdhvzrbv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvpuynol.sHtML


<!-- 参考信息 -->