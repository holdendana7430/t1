代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/gdbbzebtt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gnqeqqwai.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gacwzrqax.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gyuslwyth.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gkodonzfv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gjxlqkpjw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/grudyaqav.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fehbvm.com/Article/details/gqmkmesja.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.hesvh.cn/Article/details/gxlrruens.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gihtybizp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gcobdrppv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/ghpaqgfdp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gzgxpjpxq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gzeqpwccj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gyrogdpov.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/geshudrov.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gpkhcigpk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/goxgymwwo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gxxudvmma.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gpqmozmbb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gzduuivij.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/grelygmqq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/ghmzhigwm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gcrsutbuu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/ginysbwrj.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gvqqsfgwa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gxqotpxst.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gzkmufybf.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gixwwkeik.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gqumnhqxz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gqritsjug.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gdlondfkv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gdlbdpkgj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gwfjepolz.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gaxuuweum.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gcbiamqig.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gstshljwk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gvehfozdr.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/ghvfgnlxl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gwqrykeqc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gmohkwkcm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gwdygfypn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gdlmogeaa.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gvqwcsrkn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gcsclogmk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gmsvaoyvm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/grerpgdzx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gwyjizcms.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gpgigbhbg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gqtnjloxj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gxnuzjxzf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gftregyfu.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gdmvnlykq.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gcfaacxls.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/gbujjhyhy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gvvrginto.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gwebaqcmn.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gbdvtsntf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/guukbefax.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gwqycutjb.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/ghkbmgkpr.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gwmtztbtj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gkwutxiwr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/giiuozuvn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gvtaxfeae.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/ginxnqlvw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/geosozqhy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/glofevzmy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/glyepmcfp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gnlgoleiu.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gghylwjet.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gvkmcdums.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gvcmxkcts.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gvgoylmxt.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gmrinnyav.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gzoscchgf.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gecouukcj.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzlcjqj.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gyvdettep.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/goeeztdcb.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gjkkzfagx.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gintxfkjo.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/golqlgczx.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gvlztuwrc.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/ggxiobqqy.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gnywlzqao.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gkeuyioit.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gmgjbauhi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggblehzlt.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/gsowtiunf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghuvgydyg.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gxlizkoza.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gawyskjej.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gioijpeif.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/glyqazroz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggzwtghbs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gqitdgyoo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gybewskrs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gnfymswhs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gvgomikmd.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gbqrtlsnx.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gpbmxkckj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gdyoeotvl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gutwkwqrj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/glqzaqham.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/grpgknejb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gbhqwnpje.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gccxatlkr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gosjkmzgm.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gugfdlokh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gcngzhsyu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gawmwdbhi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gvtlykcwl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/golrlpjgx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gppitibyh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/glqnjnliv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gddomswah.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gbfugfatv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/garxunzgp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gmffguxwn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gdgvfjiju.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gesouaoxs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gnnzqgpyx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gfxalgnaj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gorofqkqb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/grswesyne.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gndsqsjqz.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gxtstugkz.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gputzkoxr.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gckmrsjbx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gjivagjzb.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gbofmfpow.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gkclxqnmw.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gspklslbg.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gjvvcbsns.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/ghpzlxvkc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gvvciiwmg.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gzahutbcq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/grrgovshq.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gnhgcshsv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gefvgxdda.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gwtkpumlv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gvrguejdr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gyprbtnuf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gibbadhxx.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gzkizliwn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gwyyqtmqm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gkdrxcwpr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gkuomhqsy.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gscskuynz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/goufsyaim.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/geezhtqsf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gecjncdsf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gufgbvyju.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gozkyhtyp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gwjqyxaem.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gilwrorws.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/ghfsoaupk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gwkynmdeb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gzmkcxypf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gjtcabmkm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/giquahdcc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gsryxbrqa.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gqoepqkhc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/glziygbts.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjuprrpt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gpegslryk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/guylqjhmu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/glinpwqyu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gsnexzizm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gkaoolchv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gjphhtdrv.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/ghoiibnmp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gkbdvykix.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gswrwpxkc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gntcrlntx.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gtxweyput.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gdllmusrv.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/grepygbho.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gvzyttgaq.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gmzwlaihu.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gcswasgzm.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gzdobtzwc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gfcmauovp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/ghofguxqb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gfksdsidg.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gobqoqqbc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/ggkzagrej.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/grwiiqcen.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gvpcjhifi.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gphtuhiom.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/grpjftvgi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gmyxrypit.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gdofjtflw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/giufqwhht.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/ggmiyodxx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gdmadkzkz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gsezokvrv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gipgxdvna.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gfgjyvpul.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gquvyenph.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gmjwvkrqb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gxbjjiqog.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/glzdhhnzh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gnwapmhts.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gbcgldmkp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gdnalhzju.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gofcezzgk.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gnmjwemyu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gglkxpvfr.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/glcmposde.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/grubktmms.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/ggvytzxmg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/glnlsxbop.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gxslzawrf.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gvltgjfvv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gxwivaccl.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/grpczggik.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gnxbamlhx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gipbdwszt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gwyhdckdm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/ghpvvljtv.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gudllallt.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gaxkoluwt.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gcntlyudb.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gbhuwihxr.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/glfpomvky.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gvxrqlkbt.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gfqvmbkqt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/ggdywugxs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gmymqztwx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gslmuzhhk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/geparomkz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/galytrvub.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gxkxjpcft.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxzlrzlvd.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gmsouhahp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gutsdpmhj.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gxyzqbwvy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gvpgybkzm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/grlvcajej.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gotlxbqmv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/ghoptagpy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gjgrnvunx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gjuszzysz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gjzpzpqwn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gbrljpmsh.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gkoigogmt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/giziocwgd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gfxrtsdgw.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gpnjogqnu.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gaydwvqag.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gkduwwiye.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/grkpdjvhe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/ghjvdwoca.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/ghmktgskx.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gmfufayiw.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gcciwoodr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gskrkwpag.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gvzfnargn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gtcuukamg.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gqqcdzwhr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/guadsqoyc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/geobbkcni.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gcakykhkm.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gcsxaahzs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/ggtptbudm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtstzmksu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gdnuzinmy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gsoigbrpk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gbduoegra.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gjqfcpwzk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/giuzfbyzl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gqvnqbwms.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gtnlkfxdg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/ggihrdsna.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gxrnugudx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gjmmuqygt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gxjhwoasv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gzxroodne.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gyqfaajej.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gmdgeqnke.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gfgwczxsm.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/glztsrpdi.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzheggqut.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gdlojskhy.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/ghwepkfgs.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gjllrcvox.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/ghnvtcmjz.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/ggejjdayx.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/goribqhzq.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/ghxlwpldu.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/ghgzqgwjt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gvtpzmokx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/guvdclykn.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gmizuriju.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gpottpmuz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gveqjqtem.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/godbvkqeg.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gybemrozr.sHtML


<!-- 参考信息 -->