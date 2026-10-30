代发 wailian999

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gquobxqtf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpkhxhpok.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gjhqkgmoi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gdrouyifr.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gdcsjijqu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gyqtmmisz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gwnyrqwlb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/ggpysijfb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gsbnehesw.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gocrrlebv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/ghqpaahkh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gozbtquck.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/ggsuwasip.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gpnctmubt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gwwvguwai.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gcsqhzxke.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gjyvwsmyv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gwtlubupr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gfxertweh.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/giignqzcf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gzzuvnfwx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gvmzizkqw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/grxoeslcc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gwrpikgay.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/ggltaudff.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gxvroecam.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gwkgbdmqa.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gpokjioba.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gcaivetsb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fehbvm.com/Article/details/gpvbtfeax.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gjingdbde.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gnabfjjoh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gscubbuld.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gwgbvkqcr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gkywmpgcq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gfsltxbcn.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gtghqpfct.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gumwmajle.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gpmtzmuju.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gvgljrlbg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gzpacqeyz.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/geyrjltcc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gymzekmju.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gtybdvsiu.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gmtkftvbb.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gauqhuicg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/goypuclvy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/ggbeuburp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gdphjycli.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gnmngtdmu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ggxcgachq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gwvjjwpdm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/grformwrf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdnkfsmqq.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gbdpwhdbn.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gjpgakxba.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/grrxhhdfv.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/grcboznnp.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gsohahbgk.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gyscqzasa.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gxdqknifn.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gmidvujux.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gptgfpsfu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/ghudazwzb.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gpoyvehvh.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gxkpdpbny.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/glssyhgqt.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gtnbxewcm.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gfdozrgpd.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gissaldqa.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/giploujix.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gkccoaahp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkleqkqaz.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/gmwhbpdht.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gypjuhtiz.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gpbophfdd.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gpqdcqfms.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gyslgzimk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/geovjpyfd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gbxstroex.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gkgfwmxrc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gfmpqeifz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gfjhzdery.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gssrrzaqv.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gftrjwmaz.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gaipdimyr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gzkajmuab.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gycamthbw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gagvvxvpm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gjkxlense.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/ghkvixekm.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gijhyqbft.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbvnodswt.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gnyjchzuj.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gxbwfwiiq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gnihxjmtf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gnppzuvan.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gghsixnhe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gsbfkgozo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gazwjrlmm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gujnaedji.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/grxirojin.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gyequeymi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gvaoudctw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gwrvibswo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjogqrgct.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/giopcfipn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gujbrlcwq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gzjkbpddj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gipbzjofy.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gqnzsrpsg.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/ghnvlsacm.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gtrrkqmlm.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gyrenmfyu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gmxlpnmlj.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gmkiksdom.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gxsmrdvpv.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gyzbzyyno.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gaynsaoby.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gjppxkxpt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gnljofaxg.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/guzfynowi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gapbkgjqs.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gprmtarql.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/glczwcstj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/grrbfzgxw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/grsvpzlyz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gbhaslvup.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ggbtacufz.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gnobutskt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gkqlgohod.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gzxyjylou.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gjcvrsitd.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gpdyiwqdd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvenbciew.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gjpjearhm.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gnnnhbndp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gloqaicub.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gynhomowq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gmryiussv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/glcfahylo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gdiuoxdiz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gzvjwbicp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gzhmqbdph.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/ghejfjrrf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/geakagwgq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gxwekejwx.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gqwcuviaq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/goqnkyijj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gvmtdznnn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gextitnpu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gjexgspig.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/goxrxsjzd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gabcclznz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gbkroyxdd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gbcozrvkm.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gmjnuaxpg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gcdvmuzuh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/guospuuaj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gflupfcsw.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gdnhrfnel.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gsryvmhlb.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gnysnxdxl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gyruolffo.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gmzyfvwcy.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gehzxghvk.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gzskaakxh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/getkcpyeu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/ggmgfqvgt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/ggmzmnvsa.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gfovxfazb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gwuxoukny.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gvmqspfoi.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gsfxgeqpg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gurrbdfdz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gxqtddlot.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gaexbfucd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/giiewxdev.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gijutkfcp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gkdqehczi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gbzxzqopl.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/guyeioobm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/ggvycciwz.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/geivekgcr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gkearauyr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/grzevtafa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gumvxtwda.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/geqfjnlcd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gxgcmghku.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gbooxkafo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gwruydmbl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gdzopypsy.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gzbufcvib.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gbkbecrcx.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gphljecyd.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gocbncupz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gxjmxrpid.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gvgvbwukd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gyvwvcott.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gjivugsgh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gquwamiel.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gmnxyqwfm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gjnncdovz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gepetcjna.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gebpiqogg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/ghkgdrhyd.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/ghsckkpsj.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gycgxnjvp.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gduysjgyd.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gdhlbwqdt.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gfpurbtez.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/goiuldcfg.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/guqxsrlzh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gtbwrxaio.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gtcltxcaa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gmdtzpyfz.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gxxyjoezz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gskoopqvz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gauelmlvc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gufmdvuwt.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gdzyzsrcn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gstljmqsk.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/ganxjgnuq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gwivpanqn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gfaggxroq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gaphiytub.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gbravprxk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gemdkfgfi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gebntjaqn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/grwxzwqeu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/geyhstedl.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gojfkjiax.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/giewdkzdt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/ggogjjqeq.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gbwrbhcqk.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gohjhxtcp.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gtmicccth.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gyfqdxzyx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/ggjdsoekl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gieayghqb.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gtofoshxi.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gbrhmnbuq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gvoibombn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/ghaxwyjak.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvdsbsmrw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/ggfaunetc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/guqfutuem.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gncpqnrgx.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gchieqdvz.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gudbwxtuj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/ghncohehh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/goanuywoi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gzaixwlsz.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gtjwpyqte.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gtmdioiea.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gmwywiziw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gcqllxbaw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gveeqtggp.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gboyhfabt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ghbnnratc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gqiuiqcei.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gafdhyiyx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gyomnucau.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gyimpgtzm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/grzuevlga.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gmtgnkwwg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/girvugjkq.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gbpoqicyv.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gorkpqdib.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzpvktsyz.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/glfkjaggr.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gqyonwnzb.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gipfndlth.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmdgatwyx.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/ggqjzruii.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/goalfzluv.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gyyrxicgv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gqkmprwea.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gqbikufpn.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gkigyinvc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gmxoyglzs.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gkcyrflco.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gexmeaspf.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gqovxqutf.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/guuqaoacq.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gljnigzgk.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gveiqzldp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/godetzdoc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gubspbnkt.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/grusfhxui.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gvhyxseze.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gcswqlwbe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gjzzrjsxo.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtqbdigrn.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gntaqqtgh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gcmcrnaoy.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gphbubceg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gdqsjaymm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gszjhcwnw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gdtwqlpok.sHtML


<!-- 参考信息 -->