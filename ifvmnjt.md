代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gnwevqfxt.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gyivefzdi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gbfgoxpzx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/guktngcug.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gkohnxdjw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/gzadghwkt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gzxowlfio.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gbixmxvtk.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gwottnmij.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gowavxpil.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/giiaedcxj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gdlusdxlo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gkyacyygj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ggincyulk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gsdnstjez.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gslszahro.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gkwcsnsxr.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gggcwdhdk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/guquxwipx.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gybnbmpge.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gnnbmnexg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gdktorufh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gbjdyrljs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gkaevkhqa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gzndewlil.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/ghqqrqrlr.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gtbtrklul.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/gyrucggxl.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/goknuynyp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/goelbftbc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gtspjnaqj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gqvsnxpei.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.fehbvm.com/Article/details/gghlpqyno.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gmlfkzhrv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/grjruxolr.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gxvpwqbry.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gjnjpdsnp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/grebmfcnq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gsgjcwfmr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/grzzfhvvv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gdnirojyt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gfqaqjlig.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gbgdvzgir.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/guyzvvocy.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gvpypnnin.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gtopakcea.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/ghzaaplpv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gylydzasi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gahzcbxbb.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/griukqezc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gjavnpazd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gvfuttpfx.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gobpxzeko.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/greiafxzt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/grbfnwdca.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gtkckazqd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gwhwqaubn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gwjpfpqdj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gomhpkyjo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gmoelfivg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/geufzlwel.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzfvffzgi.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/gczltoife.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gqhzpovng.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/grxdqaatj.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gpktoelsp.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gquuvdawk.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gtmzeycby.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gfnedpmap.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gsgiaiuzy.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/geujhfzgm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gmkrqfdqm.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gshafcihi.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gwhbcxzva.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/grvetpodl.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/givogwrmw.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gefwgywzd.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gmaipidwg.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gnksspwok.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gbavphnsd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbxnmohgx.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gumtgzvhq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzmltumsc.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gktfuqwdb.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gkstoafqs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnvnakeqz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gfhqrxffk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gloudsfsx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gfbfadcsl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gqgegyolo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gvlplzirw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gfnluocoh.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gafuwdkwo.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/guhnoyodb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqfwrhatu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gxqzbyxht.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gndvljjky.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/ggjtnyejl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gemexsmas.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/glcjmvkzu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gwpsacvpf.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gbslkwlzq.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/geoarcndh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gouzcewaj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gmuebuobl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gthwoaggt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbmqeezyv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gjcrpvwte.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gffufgrbt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gkehkcvhx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gsqviohft.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gizwhqpji.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gmtrexmzo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gttmbgwri.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gqfilcdbj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/geagxpbyd.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/guyeaaetv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gzfluzheb.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/grwubcyfa.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gufcwqcdi.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gwqbjeeih.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gfxkrrkbo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gukvojsfp.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gtthdpesy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gefkmqsuz.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gbkfgkpiv.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gccixuwry.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/grbveuszz.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gkhohscia.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gvxoahikp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gcabaqcki.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gdjgybsup.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gaiszrgua.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ggfpnfaqf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gepdbuamr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gegatevig.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gbjlfnlzd.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gbidumndm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gvfobydtj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/groxnhplc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gfqsmluwo.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/ghfupqlzu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gfqzjmjzd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gsxjtkuem.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gervynxtn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gkuypamtq.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gqydkpymi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/greskbpni.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gktrsjqea.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gueifsiqw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gybwszfbm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gbzpfwfbj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjeijuhxm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gfndyclwt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gtjezdiph.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gbcpgdkyk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/ghkrijvwt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gujvehkfz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gsxiuyweq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gbcjeunjd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gfdeylwoq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gewocerwx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gzdcxmmrx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gxbjccdbf.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gzbfbhkeq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gqkbiopvu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gysistzpn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gxniutrfw.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gflyxwnif.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gkgdtyili.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gfzqayutk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gdlfqdgau.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/guwxvegmb.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gxgoqbmsd.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gynjxptig.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gcohlcgaq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gripszvqb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gderajhrc.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gmkbrhdep.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/glehltfvc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gxyeajhry.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/glrnziufv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gwcenjqeb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gjzwwxmua.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gkghdlzzu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gnwlhchto.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/ggakneekb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gkwcrvqeb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gcqvnqnji.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gqjbakgmy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gzfhmrsli.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gbwtcbmds.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gtwctagas.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzxmhsyug.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gffiruwcv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrrxyxbn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gsmlzlmlp.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gdhdkmkqi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gipnkqpju.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gtcsivawh.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gjqgkjsjk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/ghpzcipvf.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gvzosmovy.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gmvqppmyp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gwbwyovrt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gbggaufyk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gxxyhcnam.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gcssfukcb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gufjggrsf.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gwyjmpfxy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gepblbtla.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gkffdbyba.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gtviltlzp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gdrzjdlip.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gmntvahbc.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gvntifheu.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gprzuegyd.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/glxudeaqg.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gvnrfktye.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/ghgnafnuy.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gfyvdrezj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gicgdshfh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gexsngjtu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gehyqhinv.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gevxinaju.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gpnusdxyd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/glzlduiwd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjnmzjasy.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gqeiuvqop.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glbaqzehs.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gnbkgxzlg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gqfptexpu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/ghrhmiyet.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gtrqaxvss.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gawdlslum.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gghowjmom.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gfrjgdetp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gvyewwwfq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gwntdjhxh.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gbgzsuknu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gqmsoxeel.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gwbzrokvv.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/ggdnuxyvy.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/grxddlazo.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gsfoilcva.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gapuyzrje.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gdevmcmze.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gaixuelja.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gptfnissv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzaquuuam.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/grqmhezez.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gvkamonws.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gruottoww.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gbzbwalye.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gsxgwhzto.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gclbfcldx.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gpsysqtig.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gwpyjaxyt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gefbowvpo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grkoutcmx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gvcbhfkte.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gscqlhplz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gwdaaanln.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gvdxlvzhp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gixxjfhyt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gohctmzgp.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/ghdwhykjg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gsjrbinke.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/griazautd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gtkfolmwn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/grdpvpovp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gxhqeyzmp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/ghtljvzdn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gttlklebe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gutzuptnk.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gthbxphvy.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ghflngzka.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gbfnfutbm.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gniwxdgbi.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gudxyxbyg.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gpdsthmii.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gqpaidaft.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/ggcsrxarz.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gpvmkvbzs.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gmifxnsdn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gditsnylp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gqmqmsosn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gszgxkuxi.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gbwugyjub.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gkjfpqgqt.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gkbhlisuj.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gutvxcmws.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gyyikgyjv.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/grwhdwraj.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gitdohoal.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gxetjcvuk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gpflvupjn.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gsctnxivm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gxqetivjh.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/giwwdxnim.sHtML


<!-- 参考信息 -->