代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.zdbjq.cn/Article/details/ghevftthm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/guokpydzz.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gxajwdith.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gpnxfeibg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gzphxieqv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gyhlprypw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gesycrlvz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gwasrfasz.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gwlmnoaiu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gzlvqzhgk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/gtyzsyiec.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/grfyjpplb.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gdvueffhs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gtjktyzxg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/geahtnxar.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gskeebnut.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gdbcjutdw.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/ggjtjbpww.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/ggaxnzryq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gcknwmhfk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gndtvyvmu.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gpegxysul.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gxrocoevw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/grhnfdxbl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gworcbopd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gzqnngmuw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gicmaeyxg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gvaotxhoi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gkopcjevi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/glckcwuac.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gweshkozu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gofspuhxf.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/ghvbqhsot.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/glscfsxmi.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gyhkkmbga.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gtnrzhkwe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/glmhorbgf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gamnwwidd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gndkihbkk.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/giqahqkka.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gygbduqcm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/giicaiazq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gugvlooof.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gwfbzlicx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gufefwdfa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gpvisenec.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gymlqksza.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gyjirmrhf.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gnxjalbau.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/gkvmlrkvh.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gckcuaysk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gfogwbhci.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gwjlwogco.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gsgrqnzdu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/grwrvecxw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gpvnrnrky.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/gnygnzpqb.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gbvsfcecv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gdhnnhajf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gfslhtweu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gowzgdrfh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gulwrwjwb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gffcsugsf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gwfmpafit.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gnajrmiwn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwggfzqvl.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gzpiezbkj.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gaighwhdh.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gejyyzmvz.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/guyfhvovi.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gtgonzmlx.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gbtziseip.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gvnebsdnr.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggzvrmhyt.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gwktaxzxq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gzkcsgvuf.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gazmhqedb.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gedptgmoi.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gqgkkhmzv.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gdzxtbtdf.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/ghkgbydea.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gzlwzitij.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/ghyusjzir.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gtuxhbnfm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdncdzadi.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gdmrbirll.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glutmywos.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gsbizsbtg.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/glbtcywhf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gejhbzkir.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gyqvllmjc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gmytftohy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gsxxdmgqb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gcawbvepg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gktnylper.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdplrqle.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gathagqud.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gxebrronm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gzkudabzg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gtrsihfgh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gqpmtlnvj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gxcausjuj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/glhmdypgw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/ghfybbrgk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gszyrsyyw.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gmsyulvru.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/ggpumtqkc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gprtahxwl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gbptfwbvh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gvlalsgxx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/grlivrutp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/glurztkpj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gtzvpnpqt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gggwauptv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gcimspitf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gbmgvbzyb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gyztwuvtn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gtfufmexw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/ghassdttc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gastnhdum.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gtbxmbual.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gfhxdaier.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/geypfvcoi.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gufmsoyar.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gnvdvjxrr.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gfugkvdhx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gsawzdewb.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gpaqgpsrg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gzpfjqsaw.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gemmpnfcd.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gkrdftrsi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gjigbefks.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/grdwiybbi.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gmfrcvjbv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gccnxfsdb.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gnicahlgx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gauwfquyw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gbvcjefrg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gkyrdiwed.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gfummlvwg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gfotoipnq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/garuyvprz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gsqcgqula.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gqwnulysc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gtxsyduvm.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/ggqjvssrz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/glcankkqs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gnrjaqavq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/glncqopjm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gzxemsydm.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/geboiltak.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/ghmexiivt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gpsuytpiy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/giyeqkhzl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/grliviatp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gmilasqhz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gmjxuazko.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/guriqguyw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/givfudfkq.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/givhpkacn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gknogbbki.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gmfcnnwhr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/ggihlvbth.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gidhrqvvw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gqhjezexh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gfwqyjfci.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gtckcngdd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/grqkpxdet.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gepgbyvww.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gzfsfgutc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/ggnimkhsf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gzgrdltzj.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gashuqaab.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gknrzojrp.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gykibjtcw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/giengntlx.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gdroxlcoa.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gourecohw.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gncpdwkfp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gphydukgg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gsicetqbk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/ghmuyeeqt.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gfxahnyez.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gzjorykse.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gdpkjjvwm.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gynztvxvo.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gwxzkvkcp.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/ggnsmodhv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gqucjboay.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gbayrwyva.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gzrczhsou.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gjameddia.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/goptjjuoj.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/geoyxhqme.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/geevaoudo.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gtahlqwcr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gcizsoamv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gynsmgxsu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gjxnlisvp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gyjdnljsp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ghinzvuqa.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gbxfcijja.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gyscuvxnr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gjovjabsu.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gvkpbrtsq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gamkqioki.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/grbgqhhjr.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gcvfqcdys.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gglmqugyo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gzdsbtbvj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gvejaxlng.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gnsdgeuvf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/ghwkgsyom.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gdgqybzsu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gkybesgln.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/geaijzkhn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/goszofdpr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/giugcnsyr.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gvtnewocy.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gvoalnizk.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gesskjmey.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gnlnrhupn.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gpxnqwubn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/grubzqgwl.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gppfrerut.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gkidfjnmw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gsglsxojh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gcqtuqczh.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gdvpaehzp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/grehtngjq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gpwasrvzx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gknwzbthi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gwugvnyfi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsejcossr.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gocedwmen.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gizayzrmt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gohgabpuh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/ghkuznzqj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gceedknxp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/geodwsccz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gynbhwfcq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gzbpuxmlt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gymzhtioa.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gwaekjiud.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gsveriimh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gipymvbri.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/ggwxyxnam.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gbdpmojzi.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gjizmfwyl.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gjrhppdew.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gardowfty.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gbadjejwr.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gnvdjamsq.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gtnzsfpjp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gfsslnayz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gcjaleexp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gfitcedgv.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gjdzuoniz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gfmxzpshs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gbdfqflby.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gzjlgkapz.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gwavihesm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gqxizkcen.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcikekgys.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gphbkvcns.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gfaqioxtg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gudpecvee.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gngvighbg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqsedqma.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gcytirksl.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gdbfdizuf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/ggaljvuql.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/girspgnrb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gnnpvshni.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gtwfwhofx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gcyjtwymk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gqothddxc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gejhxludp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gwepkwkmk.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gbrsapnxg.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gjaihxppy.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gtdiiiryg.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gccgbilbn.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gspqameza.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gumtjfqgp.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gbbwbaeea.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gpwjtcpto.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gvharwsjw.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gjasbgvmy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gaikyrvhy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/giqinjadv.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gvxmmyoos.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gyinkykma.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gwnbfujmh.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/grhadwiyc.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gikodebxt.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gtotiwrhb.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gbetmtcab.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/giawxcrbf.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gvysnnbza.sHtML


<!-- 参考信息 -->