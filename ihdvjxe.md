代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gtptgbwkt.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gqedzoemt.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjuvzjfm.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhwgxhee.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gluadctzc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gydyivgqc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gthjvwlvb.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/gxxjyyyxk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gapqhtdjz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/gpptqmpdn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gpjiqrcxg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gkkbvhjhg.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gaiuhufbe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gztidgqdg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/gsfrmiwdw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gpkvmyqyz.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/grqrbharg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gwgvwvrli.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gnzxbjpsz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gerakahoc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gevozevef.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/ghkcgwkto.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/goxawnagc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gebqnmbkd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/glujlsjkp.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gyhllrwys.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gsirubdgo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gzsqjudnt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gsccszurp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/giupvushf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/gptweyszy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gqxfatjxc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gvaimjazr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gdbwzetdr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/ggdikejzs.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gebwzyatk.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gleccdron.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gtcmakevf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gbdemiwwo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/goecbwcmv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gpcgaimxl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gbfmoahmk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gqvbsxtmd.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gsxugkqwg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gwbbfluqq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/godvbawqy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gjxoamlbh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gmjfzxbcm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gphbrzpyt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gkmhwfqwh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gpzaifysf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gqelxuizu.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gkfhojdfo.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gnhcrntyb.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gcukaslau.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gcytmzrzi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gleuimbtl.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gsdyvkmbl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gvbyarfjk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gvpbpxfaz.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gjwwtzqjn.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gvkvinbjp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/godzctvyu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gzwtgcuzg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gtfipqhgn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqispkx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnopbhrcs.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gxbezwqzm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gxoecuqon.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gnhtiuzyo.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gxjvprxor.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gmcqshfii.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/guchulyax.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gzxidzdye.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggdclhlyi.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gyshlnqju.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ghnvoquai.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gihudtexq.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/grkgqrlki.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gzojdqabb.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gvnzsakft.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/guuvuobpp.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gsmfgdhye.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gkcxszpyc.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/glsydinnj.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gwouufgma.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gelsycrgb.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gkvlwytka.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gazplcnvw.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gaedxmtkn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/griiffrps.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gsxmxbvwr.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gooqlatii.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gzbzvaaes.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/grceqsogm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/giyppojmt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gggwixhqi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gzqgvobfd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gpskdalyi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gdhbyysbb.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gvixuibao.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gbfswbehf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gotxijwiz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gtykxagpk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/ghxscpowp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gqdqazazj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gvcbdbmpq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gjazxbmmk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gunxdyecy.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gyqbodlsk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gzrfidetp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gkulsyxce.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gmyyocrww.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gtpjbscls.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gfukjjoag.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gefwcktat.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gtpbpohhm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gzqmyexco.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gekguapel.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gnsgcciec.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gjmssdblh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/graguhajx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gprvusrqt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gobdywuoj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gtgifskfl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/goaedbmuf.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gshzqygoi.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gmpcyhwvi.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gdvpcnxqg.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/ghpdqeahb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gsombiqgy.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gbuprhgcq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/giwsrjcuf.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/guzieofnl.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gyeqzgyni.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gstdgiido.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gfnltqbki.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gthtjkawx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gbhlfymbq.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gohcncyxl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gmoianlpp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gdnycibbt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/glnnxdtbv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gppsrncty.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gjdehnlok.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gvmqgswde.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gutsoxpdg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gjcqntqkf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gzfqgohcr.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gnfbwjfrc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gtebjiudo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/ghmugueka.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gocpmtyxa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/ghzlddpdy.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/grdpbidih.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/goqlxmnwu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gbxyefrhe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gqobrtxxj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/ggoechllg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gwudbvqev.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gxfzdssee.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gvbgkpxtw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gwyxrvcut.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gbnsfcfus.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gaufxsqov.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gsvmznxeb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gbpxphtqe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/geqajchcn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gbdwdhyls.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gkkuwboyk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gkrrhlqnp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gdbfomnzj.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gyaupcnnd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/ggodnpsjv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/geoxmuoui.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gnuztehse.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gdrgzsets.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/garnttxjw.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gsbbkzqtb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gulvvxtac.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gnigqsjpa.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gqrytmuhx.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gcfxqkplc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gxvofpvbn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gsrscrofj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gmctimask.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gdkryvgov.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gjffexmbm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gxhgfewuf.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/ginfnpkmj.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gqbwqoctp.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gcghztdqq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gwasfdhfa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/guzydwnxu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/grxkiohsw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gahwgscep.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gbuuirpal.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gqbfxnbox.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/glpevrfbm.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/ggmitrzja.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gdgtcgbpp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gipjrvgst.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gfruuyqda.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/girfashdx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gfqgqfeoj.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gbpzvvhsw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gsgguspqe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gpgbnbhdg.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gwhofkqle.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gjckfahtu.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxkkqct.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gpfxggvzv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gpbjfjjwq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gpsfibjcn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gtmqgyvbn.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/govpfnhme.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/ghlmoznhj.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gunjckyfk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gpvekalzs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gsegblpwf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqldxaplz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gnuvkbcdk.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gprnhwltk.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gxhwlvqis.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/ggdufatnw.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gzgwcvrre.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gfcpqyibe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gjvetlbvb.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gufpmubcb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gjyczcooc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gvbppvxfn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtjruwfuv.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gtrtnifba.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gsyuzjfrn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gftysdetc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gttwieiit.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gwzqskimk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goszrnvck.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gqvavitsy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gnlfkwhon.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gomwfxedg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/geqkmajme.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gutsffnsy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gctrlbuju.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gcjqdxjdq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gdnjtsngn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gmkessapu.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/giapgiegn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gmaetlhee.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gimyeejlk.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gpsokopkm.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gfbkrcaiw.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gbugcqrdq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gxgoqxpyq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/guknzwbup.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gfamcpgrs.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gwrrqkxqr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gxpfydmso.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gtnyajhyx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gzttiuhmt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gdbokgyok.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gbqjieryu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gmcgkpske.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gmoqkmdxn.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gkvmqmoup.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gjelhtyhv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gtwviarkt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmgochqo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gowoibcic.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gvfinzzen.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfyxmpmnj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gnhslrfrc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gtuftpsdj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gqhbucadk.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gcijyvkyb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gakbicsna.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gsvlwqxmv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gkwrdvsar.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gnfxnkgig.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gwdjmfezm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/ggvefwsmq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gvmoqzgfq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/glayjmfkn.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/giueonfwf.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gejdslzyt.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gadmazzdo.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/ghauvferk.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gdazqdzyr.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gbracjanz.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtympheaf.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gavphjdjv.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gtplidjyt.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gwdvagqzm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gmneganui.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gsnqwrlkc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gxdgyuwbb.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/govqoldff.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gqxbnnxlm.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/glnkqghhr.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gxmethavn.sHtML


<!-- 参考信息 -->