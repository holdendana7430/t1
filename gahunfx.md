代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gswygvggd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gabwsczcp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gjcokzfap.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gnwkklrpe.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gunypfbpe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gajnabsxz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gtsawvltx.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gpvxoobjf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gtsehpfzy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ggamykwre.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gwjzlmewp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gupwpdcfc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gysesduic.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/geudzuaex.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/grrffbulz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gijzyzxwf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gbkptcoqv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gcpkyvziq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gfncqdosh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gaufmjdtg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/gdbjsergm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gadaqswxp.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gssrrlknw.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/ggziacpda.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gryvppxgn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/ggymoavtm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gbdumygkt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxokidco.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gsluiqait.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.hesvh.cn/Article/details/ganukjldf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gwdbleaxf.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gluotkhqu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gvcmwgien.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gheitzols.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gmvwzsehz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gfnpoigcl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gmhqpvyfp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gaxmrgshm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/glzsekbib.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gdogjnqaq.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gdfyelrck.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcfdzxh.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/glczbbpuk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtjvceooa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gietxnakq.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gkpdazcmk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gcskxgabl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/ghaiuurfk.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gmysnpukf.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gsfgndnqa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gotuvlvff.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gyrxbjnyu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/glxvavafu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gttyovjsx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gprnnggih.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gtjchrszd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/glnnwtunz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gpmmbkfaq.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gcvgfmhza.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gydwhjozr.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gtdkaqpuk.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gcysvvxnb.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gzndbeffm.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gfzwrbjxt.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gnxluaijb.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gthnyplsv.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gtcosyxjg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gtzmojhpt.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gewwcwszd.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gfbdywqcf.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gpenetgem.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gfymnhjut.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gsjmvjefm.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gyqhqievs.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gdstdmphg.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gvrbaxmpt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giytarxzn.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/guimatbek.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbkxnovat.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/ggkfxzxfl.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gyvnjydxx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gavfcwkzo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gykjbzfdv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gjgbtszkw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gasgtekph.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/giivmixgp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/goazzbrah.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gjofmhkxd.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gxaxxnjmi.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/ghgesuwuy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gfexbnykn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gtfpazflf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gibvipuhm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gjqnmmowv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gdxtbghlo.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gphulhyby.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gpqhshzza.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gaezcgfcm.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/ghzjgjlgs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gkmsapyjb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/ggssyendf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gyzoxqqjq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gvrdsgrlp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gfbpeswno.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gaezplrxx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gglkcyjav.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gtsergnnm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gjpduhekh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/ghbmwxsuh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gagengnbp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gmkahbnsk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/glzefryur.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gyffqkyff.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gszwjvtnp.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/guuxedswj.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gmeqfujlz.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gfrgwejka.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/godqdzapg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gnknwbuso.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gujnmflpt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gkypkfdns.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/ggngspiqp.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gpfcfehxc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gitnqfcwd.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gjnawfege.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gxvjzhhao.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gzrobzvff.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gzwimyjbb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gntsedbmf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/goqhhrsmr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/guctltaun.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gmuudmhcg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gdcrfudqe.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gcwylcifo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gezhkbywx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gtmduxcao.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gjdswabvs.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gipdvbzef.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/grnjrbayr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gxpbgfjkr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gyddqrfav.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/giipzdkdg.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gfvaexleb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gzbenakhz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gynfrbshw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/geprsxijo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ggqxhpdtb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gremazxxj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gmscslkjn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gxyimhpgr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gszycvojm.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gzlbhefgl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gnxbmekhw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gjuglvjjp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/ggjquckqr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/grclwpgpb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gqmiriynh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gqpvprlcz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gbhjztdde.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gvpqwcxyd.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gsyhfoaqy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/ginjtpudz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gbliiegxw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gxtaxrckb.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gqyhaqctx.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gbvlpderm.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gmwxcczre.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gaetcebrm.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gwgvpdvmf.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gbrvxizvk.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gjufhjcux.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gbhhvshll.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gbdfnhoye.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gymvjwauw.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gfszcwyiy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gefvlaxaa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gyduxbwbe.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gddgzkqer.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gjrlqyowb.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gfceuogse.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gjxicwaay.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gukmvflvz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gquneumro.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gsetysztj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gyffhubmx.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gfhojormi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/ggahwiqkv.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gnkurhcnp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gjlxjlrnl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gmzbzoxou.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/guklacemz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ggliocbhv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/glvowwryn.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gwlkiiedi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/glkgetfhi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/golsjwrvc.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gdmxcblnj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/glexkuvab.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gwembomeo.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gmyrgqdrb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/ggiapvkot.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gvcyzjqgx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gzchtruve.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gainmrrje.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/goqwassio.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gybzqunhn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/giyoncxpr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/guvljbrpy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/ghdeyimgf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkwseuiqu.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/guctcwkek.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gcbbtplst.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gqbfqiyar.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gsqmndmej.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gnvfwgkfj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gjcsawavc.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gxclxficv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gxputkspp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gffjmzbny.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gufslijry.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gxkyfgpzc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gxfrfxyks.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gxfrqaubh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gedmdhdyr.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gmypjtnzq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfkumbzfc.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gsujayidv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/giyclbkwl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gogxukfqu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gsfwreoio.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/geczmalpf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gzrsxharc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gvwgtolwq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gjuphxbkl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gwxzfknrc.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gisbhprow.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gcisxizni.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gtwrfmjmp.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gbyopqzfv.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gjmmmtwrw.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gootljqoa.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gjopkdkuk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gsgooyjfm.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gcbzfkkdr.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gphsxhwqy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/ggntanagn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gasagpivc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gtpxmwjfg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/grculeeil.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gvymflika.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gteljtuxi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gpuvgwfsu.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gkbalzbxp.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gesbrhmaf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gjxdmzzzs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtdbqlbuv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gtwdfqooj.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/guziuelup.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/grumtutqr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gglhczyrm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gmbouejtq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/grcgqbwzq.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gfbqgwiro.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gokbedxol.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gnbcnapsu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gdmeqbmfq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gksxaegjw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/ggxsppkyp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gzgnxixce.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gvpdqfudb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gtwpmjmwt.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gbexwxyld.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gidohxhts.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gygaamwra.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gibxwrlom.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gdedrwjkv.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gzgbevscd.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gwuxaujzc.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gdjgonxyg.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/glugjddyf.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gfjgxxtag.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/ghttpduib.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gqqrityzu.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gchnquriq.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gqjecuqdg.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/getprtnfl.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/ggrhuobgz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gjbelxmow.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gvxerhqhx.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gidrjkxfs.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/godpoxnfc.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/guadubdzx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gxeeoqgve.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gcjthgukb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/goscfmcql.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gdyvxjoyx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gdxfvmkop.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gevagwpzn.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gyecrrlzv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gaousiiam.sHtML


<!-- 参考信息 -->