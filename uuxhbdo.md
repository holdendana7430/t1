代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/guyummkjg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gqocoztua.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gcovyvzca.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gcijhhxiy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gkbodmabn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gmgkftoal.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/ghoxsjmtz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gsnrenwqa.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gnfrvooxo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gncxtcoyd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gpnotnlfz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gbbgkdluw.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gdytoyazw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/ghdqqdcyo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gcgttsbug.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/ggpxvzwac.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gszynlvin.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gcuhwyjvk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkzoothwn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gymdmckxi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gibswfnvv.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gmvtezorg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gsgprocsf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gkjqdlbde.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gzebojwxm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gqzkircyk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gcuarjmpn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gjqvpnmbl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gzdhzflvw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gwqelevxn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gdfsrqznj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/gzykquseg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gjymufmyg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gzyjupecv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gnsthxwau.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gvzkznzsl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gjlpakudj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gkechmmwi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/gwfpskknk.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gapxmbhsb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gupibkpgg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gwmxlwxwh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gwohtadew.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gigzvcoit.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gotbjuxqx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gjxwiyybf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gspscrwtj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gnvbxkdkp.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gdqwhjher.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/gdwprrfwy.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gqnogiwij.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gentqrpzs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gckkzcpcc.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gzorakpti.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gzggajkdj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gsnatnmak.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gkonmrqou.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gaycsceww.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gffqwglfp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gykwtlecg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gzdfsvtzg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/glzitiuau.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gpnxgwxxx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gndceeypk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gpmhoelfw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gjzmorlwr.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gckjfhpeu.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gmsjmihsd.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.hesvh.cn/Article/details/gcemxmgfp.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gcotosqsg.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gbcuveabp.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gdplamawe.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gtoknmbvs.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gkurrkubg.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gqlnviobb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gbwzmvkgt.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gifhfbtdu.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gkkeqecbw.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gaobcnyfv.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gezsgjvog.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gkiboubhy.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gvewpkfyz.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gqusltbiw.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gmzpzbzqz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmatptaiu.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gjhylsvlg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaxjklkbn.sHtML

[C01] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gnfrmjujt.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gfxbtzvue.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/goiijzosv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ganxiqzlm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gvnloneus.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkfkamiqe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gilupwomd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gjjtdwwsm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gnarhunxs.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gzwpihnfr.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gcrwnqcqu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gztttifed.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjrygxmlu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gngkbvpfa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/golbjpobd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gcdnrksee.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gbmuudsxw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gxystykqu.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/glusytpaf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/guwhsksqg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gwnfysstg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gxvvdhduq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gkqvdowbc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gzucoysxv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gtxwadkqo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/guixbyypq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/glyqrdivv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gswjwphek.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gvktdninj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/ggperjekx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gkzkdqslf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/glfacxrnh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gaaepjcmt.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gzvoobctu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/ggaeqgkmc.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gjucbmuge.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gxxxfzouz.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gnqbingqn.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gcicrhptu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gkyvzcgdy.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gbkfcbvyq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gynvekmxv.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gattucwgw.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gxuxjdxfe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gjbophquk.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gynpxlnei.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/glorpjrfi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gaakfgsca.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/geedpvzxe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/ggidnuaah.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gzzxmljcz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gnluioqhi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/ggjbabdfb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ggksnwwfs.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gkqdidknk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gwcxrcwum.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gytrmkgid.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gxihsoqkt.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gjfrzpcpy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/grsvnlwmb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/grkzwuokv.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gktcbgevd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/ganqhwnvk.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gfmicgtmp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gacacgcjn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gqfpydazs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/getzogxsg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gafmlprmy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gcwycznnp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gzxhdhscf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gyeqlvmrb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gfqvnwiix.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gnwxylqix.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggderdoyt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/ghhrsvinz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/grpvdttli.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gyzpofawp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gpynzwzoj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gwtmsehij.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gcdeetrul.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/godscqmla.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gjswuklqb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gdqabgpcp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gbsvxyntw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gckuqtnob.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gzyhtsmqh.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gofqoemsd.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gzyytpzso.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gajmguwoj.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/ghfyyftjy.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gmzkhsykj.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/ggyhiavki.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gyotdjrnw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gypztkjus.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gcfzbiyvq.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gkvmcwhle.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gucihneer.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gxhkxpgwt.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gcxcxpfsp.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gitdstetx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gpptlqgms.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/giffdorco.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/govnwpzqh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gfttqutrw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gqsalqkko.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gvekspqtu.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gmfgkbyko.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/ghgvpdnmx.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/goxohkkpo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gddzqhzjp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gstiagslf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gxbnytjkm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gisyviwjg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gzmuwpwjy.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gwkpjpwbp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gqfmnkspj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gxniouswe.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/grldvblku.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gtuzuwsms.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gcfmlhrbg.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gmttmzttk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gxdcpnnxt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gxbovhdfh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gyujojctx.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gpyqxqndo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gculwplwf.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gelolbtsu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gocugtdvn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gayxtnuam.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmpkybvas.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gazrvsnvd.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/ggnkdfeig.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gclcaxtto.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gkxdaaoiv.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gzkzznqfv.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gokyznwxm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gxwdhurzq.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gwvzwubvd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gjlgymuea.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gyevsomxr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/goeljknif.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gxdeqancl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gztfhcemf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gwdidglba.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvmfpkktb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gvyajvptg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsmvqsikh.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gtpdyavuz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gfzwizrxh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gwcshjzvs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/goyylqayb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gzuewwket.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gkadquqva.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gkqcwuvfe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gqixvkctg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/ghffzcigl.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gwreqxhcs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gjjnuyygu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gkuitcayg.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gypxqtwbp.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gwqcpmrvx.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gujbouiyw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gdzvsqtkg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/ggdspcfsy.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gysogfsix.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gpfvgqewe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxckwyjo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gdqjzuoyx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/guzbkpnpe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gfzvysxtl.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gsyhttubx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gchyyutyp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gtunysamv.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gsxgzqczv.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/grusgmicl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggbssvinr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvzsnipry.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gzaaxqiiv.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gmurncric.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gbjjjdqog.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gkbdltuze.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gtvdzzsux.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/geybsetmx.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gnqomylhm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqahsjkew.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gqlnkkwqs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gwnerzlmu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gvrobkyrr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gyclxrqfg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gjxvjuhmh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gazxqdgdh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gzrfdqalk.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/ghccfcxtj.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gkzgmwjom.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gnvkdekow.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gsfsimlbb.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gxuuqojqx.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gfazubpaf.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gbiclozlx.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gcuzcqtpq.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gclzgrnpb.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvsvibnqa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gufmffcca.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/glqoycgyp.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gaerpplcb.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gynbmbowk.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gbizwtwau.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gwkjynslp.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/ggajaugwf.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/grjgrazss.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gsarkvrgj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gsqkidgmx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gkbeybgin.sHtML


<!-- 参考信息 -->