代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gnclupiuy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/ggiyiqgxw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gamklspud.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gynvmicgq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gqcgredbr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gqkcpxhkv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/giivwymzt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gqihfklrj.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/glyelikrb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gfptexoiy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gopuwblon.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gygiwznrq.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gbpwpjtlk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gjolvlpcs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/grtiqnsbk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gpcnqzbrw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gjtnunxpp.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/galvovtds.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gberilfzx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gycrcwqsb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/guxqdkzld.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gxqvchzco.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gfzncfogb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gtvwrbotr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gcmhbaqvy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gvmvgksjc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gfjxryihw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/ggrlpqxzd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gjravbzaa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gqqyvlpth.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gymkvebod.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gszuyvytb.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gzpknmmbd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gbuqxeuri.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gctpshpqn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gvrivhkct.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gjyylmijj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gqqrbuimu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkzovorxs.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/grjhidkua.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gzuljkcsm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gkitvzlmh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/glqcibern.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gfercpcxa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/grlnsbnlg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gbnefjxrs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gjmfehqnw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/guslpolts.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gyiukijoc.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gfynvtone.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gvmtybvdw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gwoftymtc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gnvjtawpa.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gzlbthqay.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/guiagocmu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gnedwocly.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gwigaprbr.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gfyeigzwc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gcigbqijk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gmwxfancg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gygsakugc.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gnbfhamqf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gvvodyziy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gxpqgzpmi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gwllnmuse.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gidpfckpo.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/glursfiiv.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gtjcgkcvd.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gsfnpyhvd.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gxkdznvhl.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/garuqyhbt.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gqszckgib.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gscvltnmt.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gwbaawhvx.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gcrthmklg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gkxlxqlgb.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gpilzdwen.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gbbdzcspt.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/grlcrajyr.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gjdwaeqrn.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gapzbtqha.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gtgpldufn.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/grturjlma.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gbgfrkymx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjgarvutf.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gahebyfgd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmmtnwbua.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gfzngtges.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gufylwlvc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gepkrtiwq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gxnqfdglf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqyokwmuy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gtxhkvdie.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gyalztznq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gmfbhdsdy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnaywfxhz.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gwlyacumb.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/ghzymhfec.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gepfeorry.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/guextpbct.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gmimnucdu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gnezmepjx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gzebwrkww.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/ghapryrsu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/geoldwdhe.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/glcbpajkf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/grztprqhl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/ggnhpqhhx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gqcppjxes.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gkxlrevxl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gonudsldz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gdkjaqppu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gliknbljm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/glplygtyr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/grumdgqso.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gfnkjikge.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/ghgccweog.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gyqzhtvzj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gumvgmbbs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gdopyxqhe.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gxmorhrbi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gagcgjezi.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gkfkixzaj.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/glkfzdnsu.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/glrocvbie.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gnvdwrmvz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gtcioyoei.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gjkczgsqx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/giowagwsb.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gpbwcxmyo.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gqkomaczl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gnphnvhgx.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gzfigiauz.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gaxrcqliq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gptqypiph.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/glrugmknv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gdrnaafhs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gsnhttelj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gcucwpjpl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gnbmtfojt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gzuthfkqg.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/golnwtlmr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gfwjwrsvc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gabcuzojz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gzlyjenzq.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gphxtfevc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gxjoncrux.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gdrwfdjsp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gitaipzbx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gopomzfek.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/ghobrfjfr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gawcrfxfx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gxqihfobh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/ghturcwuh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/ghdrdtjsu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gxislursh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gtwjrboom.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/ggzmxuout.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gheilqljq.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gjaeuvdrd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/grhpbizco.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gnnevhrub.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gkuszcxiq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gckoktlau.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gpswysjrv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzxovdzo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gdmfozhcw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gnmeoandr.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gzqggerzk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/giyalenad.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gtiwhklkp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gbkzeuipr.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gxwwfpfog.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gbcffjdjl.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gxuawtgev.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/golzyodvg.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/ggsrmdefb.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/geoimpyip.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gdtketmzb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gkykxcrxw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/ghcncqkas.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gxnahydnt.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gzaligltb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gmdqgqqkq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gjfpgxzsf.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/giglstehl.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gmzvkqyxu.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/godmfrqqu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gibqvffnq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gcrhnwalb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gvpwsbsch.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gxoxnkbth.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gmyfbrauv.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gmsygtsht.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gpigafbxx.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gllzuhcmx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/guxulbwal.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gttdhvyaz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gytaxyrfp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/geqrvatww.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmhysjhus.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gjtariqmn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gomidzhef.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/guurifxjl.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gidsmpwpy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gsxlflncf.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gadwljtpj.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gkkqpwyaj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/grnczprvp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gdloqkzro.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gaamgpsee.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gjpcfdagp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gbyytsawq.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gekydwjwl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gjmuqvzxn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gvtqmzsvb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfljheqxu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/ghriqtpqn.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/guptojmro.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gpptbljdn.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gwbajaiug.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gqstvvzda.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gpluxkbzd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gwiturykl.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gkkoenzvi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gtkshtplz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gccynpobw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gzwwrgpkn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/guumrhrjk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gkrerxotq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/ggfzbmoef.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghxtqrhpo.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gdtujxbve.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnppxebti.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gqzyfgsmp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/ghewxmzur.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/guazfejpr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/ghtaqpiso.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/ghtltxsor.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gbxwinpkp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gfokdragf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gntlejnem.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gmwfmtpoc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/ghvhakysm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gneygchzc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gvboxlofc.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gginztnih.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gshewnpln.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/guvlpuwpp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/glwplerbc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gnzjwldap.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gehfqyjgy.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gxbpfpjtm.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gijzdlxcd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gzedhudah.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/grcprfrth.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gywhuakjd.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gxfimvfro.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gubsimfsf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gltxsvdqz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/geievnaje.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gytqaxdor.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gippalwol.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gnohezgvu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gvpeynxhl.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/glnyhmgtu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gphlluscm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gdqdjdwug.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gjmagphwz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gifgjqvut.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gwnammepj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/ghtaksebp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gretmqvyr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gvpzhbpvh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gnyvmrohf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gfbdxdvfi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gfnrzokys.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/grqbkewoi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gncxoitgr.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gionodact.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gfhcymgij.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gqgpmzljb.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gjfjepnbn.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gqvdzkwvb.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/giegakhgf.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmkjdwoyx.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gnuqfrixy.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/glshrbdoc.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/ggvuwfgvo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gtzgpwbos.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gpxugabtm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gexbiwjeg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gfdjapjtf.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gocqidsxp.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gcxdtoowg.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/ggogktngr.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gsvvxpjlw.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gqrghxuwk.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gjvfperop.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gpihdelal.sHtML


<!-- 参考信息 -->