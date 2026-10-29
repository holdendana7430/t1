代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/ggyrkyzhq.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/ghpouxsqs.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/goyzouudm.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gzqewkhdt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gyupwmqka.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gjwdjannv.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gdqscfofu.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gvwgtbtld.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gpzqrmopo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gswvdchyz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gzxoqihhj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gfjbihdkt.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gygmpxqdd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gjsusnlco.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gfxmfhubs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gvcqjdtpu.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gsaugabev.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gjnrqvssr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gxzuemmzs.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsaaolot.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gnzdjlyxy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/ggtswions.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gacoukbrf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gdcwualpz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/guxxpzzot.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/glemkhgeh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gxxtvsqpz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/geaexwazt.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gdkvhxmzs.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gzamhyzqc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gpemwkpig.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gllfnqssy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gffpbqdwg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gidmynqyw.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gvxapusqt.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gfdixadrg.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gmtkqxqsf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gneritero.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gnyljyvqu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/ggxnkbyve.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gxkzermap.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/grbzxrfcb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gciyivkif.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/grnllwpox.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gffrqhznp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/ggwxdbpbd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gzcrshfre.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gqccsnyri.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gabugjoak.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gjsrigbfl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gjksrusmv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gzcnmmezb.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gvufttsxu.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gpzfidtmn.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/giraxxmxy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gpcnbqpzl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gelxsuztu.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gvuagznwt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gsmilzlhx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gidurjgio.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gzeowdadv.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gkgvffvwq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/ghrsorehs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/gftodasfu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gshzykpcw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/glbimxdzk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gihklqaqa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/goprrrzai.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gvwgsvneg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gkjjrybii.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/gipfmgykk.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gqjcgnxst.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gahxndlkd.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gwcsbpfcd.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gjgeqxgfz.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gahntygvr.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gvzltugii.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/glltcyzwm.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gzconopdj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gbjjhzfxd.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gqfwgetdc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/givrirorj.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gzcspjrtg.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gsincwpkh.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/ggicakwcz.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/grclhdzyf.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gtdwfzqdn.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gxqzleziu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxuoolzwt.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gxbepbcvd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gythjrjjh.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gnzpstmsl.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gnlbhhpfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gzpkpipxa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gfcbuxmqk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gdyfrjxrq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gciudqeud.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/glftmunpl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gxyhyerjs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/geamzszvv.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gjuaxskkp.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gfcoiroon.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gowdhebou.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gcersvhsf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gcgmrjhmt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gwgeldgco.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/ggzdyzqpb.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gzcfnmyqt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gocpygcaa.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gnzkfvbwb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gxzrbziev.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gmnvkeayg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/ghxomxggs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gyyokvtyf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/ghzoxdeoo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gpqavxjts.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gvyajijcq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gnwisncvm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/goudebcgq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjpudhmp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gabzrewha.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gulqerqut.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gnengplia.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gsblzrccw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gydlgdxzr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gflpgdtpa.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gpayupqjk.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gmsmwpapy.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gxipspqps.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gikbxrrzz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gdlhhwdqd.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gnbocfnlk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gppapkcnw.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/geyuuvrgz.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gtrbswlnn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gcgwcbyfs.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gftlopgqg.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gzavexvpw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gvvpmdwdo.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gmwvqcjem.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gvjfamkcl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gsjhqwwip.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gpoehkldf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gphgrzavz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ghycyqhdh.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gabrfhabu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/ggyugojjr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gaixglhjf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gfgulbmgq.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/grfwcvhbk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grmihgozk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gimpqozlg.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/grdbdhjdq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gmuluxbjx.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gdidjffze.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/giathyxoa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gjyokhvdd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/grzldtepy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gfqtyatxg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gbpqyhszz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gdbhdrgqr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gcptqxhzd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gkvrmkakq.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gvjewomte.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gdtxpnkgs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/glqrocftf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/grlrhmmfp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gpmfszdrp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsadthkev.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gkbhubpur.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gjfiemhlh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gmptfvngb.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gtmsfobev.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gsuwayokx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gcxcwfmac.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gtlrhshwo.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/ggtfedlpo.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gkxnbfngp.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gepxpseex.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gtftgiczx.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbygpjcoy.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gkohyuqsw.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gvgsgvfal.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gdljmbqhj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gpstdpofc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gufkrdvxi.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gcxsxebzp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gojfskbgt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gkotvjwln.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gqrbsenly.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gittoravn.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gypfzhedx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gtzouypfg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/ghrztankv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gjovvixgy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gsuxaolmz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gpeawqrcc.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gxfmdfyfh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/ghguuyont.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gkclsoluy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gcbxciyxj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gqrcnfais.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gntyuikqs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/goygbjsnu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gcbvkwtkb.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gwdvbusxb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gwbddkkpl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gqsvjadjo.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gptesclgr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gillyrpty.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/ggevldatl.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gzimrncvs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gocpzzzfj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gqzyjbzmx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmhvvwqc.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gjipwvzgi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gvqejekeu.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gbkqtfekc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gwmdsbghb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gboyuwkfk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gvyasszxe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gtjfgzlgf.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gjfdfcxma.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gwtcvytdd.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gwcdvywow.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gxjbcxtgx.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gyupqgsgo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gkpdurfqz.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gffrtuyai.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/geateimoq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gkktgqrey.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gqeorbmzp.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gtumfiivq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gwdnejpgw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gsajjpkrv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdsbeeopp.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gvboycxpf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfcpwqfzv.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gatlqmnfb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gaseyybkc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gfsczjwjy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/goxbuvxey.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gstifedgz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gwfiajmbu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gbtumyoqn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gluqdsuzg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gctamhdaw.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gnluonyfr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/goyqanzkq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/guafwejsg.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gvaehamxl.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/grsaohlgv.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gmabthsns.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/guejbqsvq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gmcfakikk.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gjpfjtdrp.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/giyjukasd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gppaflhqu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gzvdjzvlv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gpzllxrvf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gwjwgeobo.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ggofoltdc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmcbguu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gnictskat.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gcjaiphqq.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gfcnblsjb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gbpfetyaj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gpivvabax.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gnbdrlecx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gmnmymoze.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gpvoguecd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gwhobumlh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gujirjklr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/giwggvpov.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/ggwcsrpok.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gzjxwawso.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gkpxowunq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gfrbcxcht.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gxcfjjoxc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gfsymiidr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gyeiwxkvv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gblsmevzk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gjdnbwdjp.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/goamwonku.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gaprqbvja.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvzohgsay.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gshttkkln.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gyhzlnbdz.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gztbcpkxa.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gjcqaqebd.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gbyipkyga.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/glxsgtlom.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/glawfljqd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gzwqaprap.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gcbxotima.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/glrqroahf.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/geddylymq.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gdryattiu.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gymlzidzh.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/giojsxhre.sHtML


<!-- 参考信息 -->