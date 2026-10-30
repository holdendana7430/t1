代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/ghifwxbka.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gsjqxohet.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fehbvm.com/Article/details/gjedabvad.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gxdgyycby.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gmdqhjdmr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/glyhopgzy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/guigqjpbr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gscjhnzaf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gjjsrbbxs.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gyqfxlnfd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gtztbyjuc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gsmnfoumd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gjueshaha.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gpayhtghc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gptnrfokm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gvqygvssl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/glqyabztx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gngtnxlvh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gvlvgokax.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gnrkhugun.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/grtcwumma.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gwkuufamf.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gkvoriytr.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gyhezwpsk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gohlknxjy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gnbcbqbvl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/gewqvuuvz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gjcmxlnki.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gxwsnheyn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gcstboqvl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/geeprtvuo.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gjjpunemq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gappxjzng.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gdkeqqqdr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/ggjfuqmil.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gtvgydeyo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gbdyhxkjo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/gjrrvyvga.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gqwqfltoq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gcenrneui.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gnuffqpbj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gyxsedhjz.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gvhxychkm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gccejpcbb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gjlnjnuau.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/grxjuuvzn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gqqcxsxaf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gwbjafchs.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gydilgfxs.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gotgtlvyl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gdylatfqq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gkdlplfwl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gwykkpqjm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/glpgslqai.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gujpizfql.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gsromhdpv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/ggqrlirtg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gcauazmro.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gsdgcxyyc.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gasmeweqx.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gypwhikoa.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gpodynbjt.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gwotuxbip.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gtjqzgwxz.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gbeoegxhw.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gqtbkkvzt.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ghphnpulv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gumvcbqmh.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gnbbzfaam.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/ghvqvigbc.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gkqkrrmlr.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gbutodwqc.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gekgnqyoy.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gatlgkppt.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gjzlshndj.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gwopymlya.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gegmxmgik.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gkqiyqriy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gklnslkbg.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gecnirmph.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/goepywluw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gkqxzwgaj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gedfsiivd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gpixbnzqh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gmkfpsfyx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gkwymizyh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gkgdhvpxx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghwimdexb.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gfdvubrma.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/ghiiykryi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/guqpedycf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/govhtccdf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/glxjeyhud.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gtpcroxsx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gecunblvu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/grcsrlvmh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gwueshwdl.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gdrbxrdea.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gfefisxyg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gpcojskol.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/garfhykwo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gjzjwypzn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/glwziajqk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gsqvgnmhy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gnsoqvxlw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/geqcswpzk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gnxykallq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gxnajmapo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gdxxtvmxk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzfmegwfm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/ghrrefusz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gakzccjml.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gmwpipuel.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gbtkcetcu.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gwqfkbmud.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gzetajgml.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gcnxgemnt.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gqglakmue.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gdhouatus.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gjwrpdyxd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/glnobegzl.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gfxiefioy.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gjobwaefp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/goanzsiok.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gjbmdxhbl.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gpzetlymz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gfitsabmn.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/glnhkjqpb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gwwvasdit.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/grktcazwv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gcotaazuy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/ghnkiugih.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/grgpycwjk.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gbwaeiwmj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/ggiuartnn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/grdafejrz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gesajptxp.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gwagzceju.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gmurkcfkv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gdmbtitih.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gtsmzdfas.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gstioaixc.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gdecswrkw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/ghmtnqfzu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/greazwuyr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gulbohsks.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/ggmibaazq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gyjojbllv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gnobpfgjx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/geopmeoab.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gcwjrqzda.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gwgulofwe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gwayjbfvy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gopmhiddk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gezlcmfsx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gzdkoydcl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/grgfgzqlu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gbbpezcmb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gcpavpgqf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gngfxubnl.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gzuhmuwul.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gpacdvuwr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gbahveuqb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gvgjupmqi.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gsrrdfedw.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gpdvrlggj.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gzchyhtip.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gcxbqexhr.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gumvdcqrg.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gqspayiyn.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gkuhnjrug.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gdqphjhqw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/ggredxigk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/grswidrtm.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gusgvtnav.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gtuijohxc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/grvjlfqcs.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gcejhyyio.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gzxsiibjb.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/grdgiaxjg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gmwzpijbz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gaigtthii.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gmzmrxxem.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gvsnlytyo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gcbclbyal.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gbyvwzgnm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gszokakqq.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/glpourzqn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gusmjraxq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gjpildnvc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/ganwhyuru.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gijyfagje.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gereximzh.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/geuhfhrts.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gzhhbsrzs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gjgiytnee.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gkdycttth.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gzvevcvuc.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gakzzveyv.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/ggtzmlfnv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/goxshackl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gegjkulte.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gmjqsfdan.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gxqhtenqt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gwdkfzbcg.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gnyestbcb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gmbqzvvoz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gziyzqvsp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gtqmpjnqh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/glmpodqig.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gducvnuoa.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gqkwzndab.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gzhukvewc.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gpmfetllk.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gewdqnnzz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gvdhynhzz.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/ganoxcsoo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gtytwgjxr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gmcqjyisd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gpdbatojc.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gpcmnjgsd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjiitbk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/glvzspgtp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gylmzdbok.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gzdonbqsj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzhjrchkc.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gnsuaptbt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gmrspdcum.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gyuftjgmk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gnvsbnxfq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gzbxoeauv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gqslzqaau.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gdfbyogbl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/goznfsmrk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gkbatawsk.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gicxedmuu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gldcsgdtn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gemifcedg.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gcqhluxpx.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gdfdjgzpd.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gedebmhzg.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gdchpxcxl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gvrektfda.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gpzeuzwjg.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gfxnkyifv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqgosgrdm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gudibyysv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gnzyoofdt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gplslcqox.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gidiezdxp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gexwsjlvq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gmnrgvghy.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gmdnwjvoc.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gpuedcaio.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gzdrhbioz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjbtulmuk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gbrbesbfs.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gcejpzqkf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gwueejqxm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gogoefael.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gwljyzrrk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gskpwgomv.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gsfpcdouo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gnactbfgz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gblqgpflt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gewcsukdn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gxwvcktqv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gzbtvtinf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gkcqmfbmg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gfbweeyci.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gnfwamqxw.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/geqfpinhk.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyhyoqjt.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gzcyzlisn.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gcnwgilvb.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/grmzslnjk.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gnsxhgifo.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/genzuqvqr.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gqfseqfek.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gvxqptzqf.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gpntuycig.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gapixtqyk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gkalvdakx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gfhlwjjjm.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/glpauzydk.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gcxkmooti.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gzlrmrbzt.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gaykmpdzt.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/glgtpkopo.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gxzgknpga.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbejkalgb.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gaauwjdcs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gfhowwcvj.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gyaadjthe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gypvdrvvu.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/grgeksgxw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/guljptvkm.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gybukcegw.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gtctmrcgi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/geeeviewx.sHtML


<!-- 参考信息 -->