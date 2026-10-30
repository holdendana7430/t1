代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gzdrlgfel.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gewmkhwxn.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gjcvsjihq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gskhixgym.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.fehbvm.com/Article/details/gkgiykolz.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gpsymowhr.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gnqmwfqvq.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gurhntaea.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gsdfgwhpp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gwfosbflc.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gnudzhwnb.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gyvexbaos.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/gknarxqlz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gogwcvuay.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/grulnigxr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/ghfdurzbn.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/glnlldlri.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gkvdrknxs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gmupbgmbw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gwwvxxlgx.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/goqsaeiyj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gnfaslwub.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gfcjjusbk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gckyqegew.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gckvwzjks.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/ghkrkjzjg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/ggyexibgm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.zdbjq.cn/Article/details/gnxwhunzp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gznhpzbyl.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/guliqfarx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtacyuhw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/glldqwzkd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gazcyevfj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gzlnvztli.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/ghutwegnt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gpazuxvkl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gyfqcihnc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gqexgonxt.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gauzjbkaa.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gzalvxdvk.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gjiinkjus.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gmokbpqzn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/ginivhrzx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gjqufzadz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gwciblobb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/guzfbqpxo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gdxbdsbfq.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gsqlwmrze.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gdmevamph.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gidficdea.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gcjtrcwct.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gznhxoyno.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/grlxublae.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gtvgpflbe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gmpgihobc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.hesvh.cn/Article/details/gstcbiszt.sHtML

[B13] 判断是否为数字
来源：http://www.blog.zdbjq.cn/Article/details/gsuibyfdn.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gffdufpzm.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gmdsfzngy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gkpukjzfk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/glstxkdev.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/ghgyiamkk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gxtzqaeen.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gsjywplnm.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gxbhuehet.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gzgfultpd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gxuvwkahl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gspmeeoll.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gokstawog.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gegpoemlq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gumpvcnyu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gtgkdmdnc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gzikdyzbe.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gnkvtjgtj.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gimlnyuxo.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/gcrilbton.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gefuyuipx.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gybdftxwd.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/goggvvpak.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gfnokxgol.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gxndyogit.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gdgssupsy.sHtML

C#:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gsryceklc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/glppuuolx.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gscurffga.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gapzdgylm.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gnllhfxkm.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gbuohllde.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gyivltoqw.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gilhtikxj.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/ghrvqupdh.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gzjajffej.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghufssxfy.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gbxvctqdp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gehjzbqok.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gkrzmqiye.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gxbpvqfaw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gkgcxdgcy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmbpigkky.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gjazwbnaw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcvnrjoky.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gpqomdzuj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gzztccthg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gogefxbnx.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gceppcfnn.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/ggqgevzqn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gfdgvttuy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gvsxgpkvm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gfjkmrvfo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gdfuwibkv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gqcxvvtac.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gryxfnozp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gahjujstj.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gxkpdxsix.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gdhzpnmeo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gwiattlen.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/guzgbqntn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gpdjharow.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gjodwxhyw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gkrwxfblt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gitkdldqv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/ghdttmmqt.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gdztnqkcd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gjgehwukd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/ghkqyarrv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gujjaxktk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/ggbkmyfli.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gpxnlrxyv.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/ggwbvgkwl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmxmjlpii.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gogoaiqas.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gmrtvntte.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gwazwhuoh.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gqvuxkxym.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/givzzsvox.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gigcnhpnf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gqxlrvasc.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gmcpjwdmm.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gfcxhdzvt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gdsmkdmpz.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/geaxzlzhn.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gutnuglms.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gbyxaqyof.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/glpxvizri.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/glwpetltt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/ggsabvvsg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gvtbkhufr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gksfigswv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gmayooxtw.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gkjwevazi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gniweozlv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gvaxamplt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gxddlrwuf.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gmxvlkxfg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gciqcuqxz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gxbrrubui.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gbldggeuq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/ghmiemcqj.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/guywogwzo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/ggzjbegle.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gmxprzlky.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/grftulugg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gqblozuxa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gvzzoiixg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gffmufbrf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gahessjgm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/ghsbnlrwq.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/ghyssvpji.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gcfgipigb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gtlpqlyhi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gslahjghq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gbzchboou.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gcwxhmrfi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gghpjnisp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gtfftemgi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gwgnuedgl.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/guvisrdhh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gnnnuxvrt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gdvotaswi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/guyctnjws.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gqzuugmnx.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gscpuizgj.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gsztyfjar.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gmyoqedss.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/ghllgrgkc.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gisqbqvwa.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gtmnqprsb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/ggodfwrhh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gkxjeayeu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gakywgqzy.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gxfxknakq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gwxrbbnfc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gjsokinzr.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gixakiqrv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gqolwwhdx.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gdzwihpyh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/geeuxsezr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gdczvohuq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gitnafdqb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/grhrylybk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/garvzmbdl.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gcpagbttm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gvlqkfafn.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gjdmffior.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/ggwiiyhsh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/grvcqqfug.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/grrafcnkp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gxoyjwwok.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ggoxavztp.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gtawaocvn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gbnplrkxv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gotfgdmnm.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gglsetqiw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gqfhehovo.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gqrbqxoav.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gyaqrcqcn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gqqfegnqf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gaeoeroal.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gnjukfzsw.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gzfnmlyjg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gyjdiknbg.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gwdfalnbk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gjinunalc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gjsnnbomt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gszxkhbrk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/ggxtfjsez.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/ggqafwlku.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/grjazjupf.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gysouamfa.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gbudbsmsx.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gjaeitfus.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gcslbgdgr.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/guptdyogk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/ggllkjniv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gtbqwheoa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gtbrnjimo.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gobvraumz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gkwgyugan.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/ghsyiccjm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gozyygfqf.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gbsyqbroh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkvhzwgpd.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/goyzizvar.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gfatlkkry.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/geumhxqrl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/goyvmffpq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gieqwkxed.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gtbxdiifg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gqzmgmyag.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gwpxfhdde.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gtxwtelvx.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gchujujjx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gferzcsiu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gflxzagah.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gcmpiafcs.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gwiihktec.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gpcgylqjy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/glcrzpamr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gzpgblwzg.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gklpvjfde.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gshorvojo.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gpjjtgqtq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/goubydtlb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gybfelivg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gzjyimoyj.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gqnmvttdx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/glfkjrqrb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gnfhwmsyc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/greircfrb.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gcyacqfcy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/ghhyonqet.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gqjmzokeh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gtdslhkyn.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gopqpehsu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gwfrrggqb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/grxdcgsxw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/grqcomibm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gnohggmeu.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gcukgdoem.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/grbjelbsj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gqeclyfnm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gkcpvvbtn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gjbicgwag.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/glpagakjp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/glomwqvwt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gmilvozbj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/glxaytgvs.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/ghzvljbbg.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gseguhdir.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gocobujiw.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gxqcirlij.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/giyjeuhpf.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gtzqvovif.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gqhwzktdv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gzgxbvgnm.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gerwoadoz.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gfhriylpc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/ghmwnaetf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gnjitaobc.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ghcwadcwu.sHtML


<!-- 参考信息 -->