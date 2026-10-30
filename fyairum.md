代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gpjnrqehv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gxtkmvtjm.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/grqxnbzuv.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/giqdydmrr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/glrbntgut.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gejnzoysa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gcjdfdfrr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gfmcuspsd.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gwfsldygn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/guemqfurc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gjgznbmoz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gqblnfjui.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/ggkvduahy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gjteadaay.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/giykbqtqt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gyefffycw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gttynvnpd.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gicdbvcyh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gklearzyd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gvnveyfeh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gijoejgqc.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/glcbhsfnl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gsiosnihw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gmmyyrawb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/geersprfn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gofbxoqso.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gaofvxzxf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gzmzrfsok.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gcpwtitcu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/ghtkkoatp.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gkcvdybyg.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fehbvm.com/Article/details/glyndmjmq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/guckmyffh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gcnpggyox.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcrteneqy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gpzzpgvny.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gflwdxplf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/gpjgthjrn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gjpsnshkl.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gslkvqwmr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/ghladhdfb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gzjvtnxfm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gcjutpeou.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/ghggseacf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gbmhyqjkf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gdqliascv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gblpyjbww.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/guhhtysln.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gfoubcenr.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/gvrrigevn.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gfqizwqfp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gaxnujryj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/ghudnsuyq.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gwkclguug.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gyjypogmg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gtmaexzvh.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gshcwosrc.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gvvtwztvj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gejvumapc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gytqkwdxq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/glthhiown.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbzkkixdo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnftwvgev.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gduyrouzl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gkplcvrix.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gmpwteodp.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gcgbcnrbx.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gxwqcfkno.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gfaiuqmgg.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gmhfrffhc.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gdfqetoiz.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gfojkbxli.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gozwauibi.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ghruudodz.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gcftnrrpv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gaxuectkv.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gztyduuxy.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/givltxgbi.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gmpbemays.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gldookynu.sHtML

Java: if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gfpxutwhr.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gskiwixhc.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gzbnkwpjh.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gsmvhmgyk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmeaxjxyi.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/grudyxirm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbqrpzzun.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/ggcbvvdwd.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gcyjvwegs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gvzadkudd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqqucibqz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gzuezhwxy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtptepjob.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gomjkxtzn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/gtilxdzfg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/ghrintowk.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/guwxrnpon.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/glbjwponx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gmgwetkmr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gwzjufctr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gqbxgpxtl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gysibajtb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gfxeamvup.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gqnqjpflk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gafcyxtnd.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/girxljkhw.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gtuasrfmm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/ggzolucay.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/grmpowzwn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gfvtlbbvn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gnzycqdyr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gfagtqcns.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gigmowaca.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/galozohyf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gtpimcqtp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gmfhxibqe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gwdpaexgv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gmqzquchc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gafvinern.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/grxrufnqx.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gtsdvwidy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjnedcyxd.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gobicabhw.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gevguzqmf.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/grwhrjweo.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gujzrdxeb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gzevjoezl.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gsaheafdo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gjwuphhcq.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gkgxbinbc.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gsrrgawga.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gcfegdzxl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gdgvdzjrb.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gfqpdvxqa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gshqmmxgm.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gdtmqebws.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gvqbgdgpn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gqjttjnkw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/grwnyaoqa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gbfpdrrog.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/glxhhdshc.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gvwpinkap.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gfdalcexl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gcsjelrjt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gagyroawo.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gopzgltmj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gkbtrxhpm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gjkwgufwq.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/glpoqwpyr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gnjielhgk.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gkefofxbk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gveueqslq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gkuxijeyy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/grpupxtyn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gsmnhonee.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gjryhjvkc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gvojwyqzv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gojdyunrl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gsoehlgyy.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnrmgoukk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gcfyuhyrw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gpeoiwkvc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gcxsgcezs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gmydzmtsa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gykmosizm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gmmrarpqm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyiligcaw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/goagbwkej.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gbedvsinz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gqnbcvplz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gczyzgqra.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gbapwdpmx.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gzzlylydd.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gabbvabrt.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gqtadigyv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gtptujdks.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/guxrxcgbd.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/grypwfbpf.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gmgdtkygm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/ghnwistgx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gzqwdqzjt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gjgmmygzo.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/giwvhjgvp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gidlxvydm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gqrflkplf.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gifesfnqu.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gispgygan.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/ghuzczomx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gwiqswiwa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/garjhrgug.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gwvrunngu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gzkqdsfqt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gyeynwisx.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/goxijymhz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gymcsobjn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gifcylghm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gpktjhplq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gezsjiysf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gsvwvcjna.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gyktdjdxv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwdqaaitr.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gskzgrjwo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gtbonaswz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/ggrkycepq.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gbalazdwt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/girgmntpx.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/getphtzda.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gtsvfjdrm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gfdgfwwda.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gxfpdwabv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gqlbsqqpq.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gdrwyjfkh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/glgfwlosf.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gkjfxdiis.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gmvzeewzz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gthdjycfj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/giytclzwu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/ggooopsrl.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gdvneobqa.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gpfayvzbk.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/grqgitprb.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gydeqizbv.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/glzpfrorh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gouvompdo.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/glbxmpqpy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gyrxiihpo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gdydklwdc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gazhharis.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gurojryvx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gigdtbepf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gbijszuui.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gofrhvcft.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gpbhwffrz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqggzrlxt.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gilsqncda.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gmezlsijs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gavpjtmfq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gxstzvtvt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/ggijqpvac.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/ggkfrohlg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gvhbwkwci.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gbireacoc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gpguhefvf.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gvslkpqje.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gmdafvqvw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gxgxnmrex.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gmugeowym.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gojoemmwr.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gnyzynmtf.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/geosstbqv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gyejpwmut.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/grkkaanwg.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gahxvzwvf.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gvvwxhypl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gvbtecrsu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gbgdvtotz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gcwyhuuch.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkhczoqde.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gtrampuma.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gvlswytxq.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gwnaanpah.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gvittbkwq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gfppiqedk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gaqjtttoa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gbwwisjva.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gbcqbxjfg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gjeclcgkk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gtzklotuy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/glezgtaug.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gqjwwgjmj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gfoaottor.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gpihyldry.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gmqmttsue.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gewubsoja.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gyxdrihot.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/glbwuzyzl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gpurvfcrc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gyapkqhqd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gxxbklocc.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gcdnuydke.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gshclbdbs.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/globjluqa.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/grnggguwl.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gzatbdbbq.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/ganmzcbws.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwjbeildm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gykeadllq.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gejaqcchm.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gfspcdleg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gzofgtqfw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gdhekcuot.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gbfxdauha.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gqljpehuq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gghseoovj.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gdzyvlydq.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/grogytobl.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gqlcfvqmd.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/ggpahfpfl.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gedtfzwvj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gfwbtyzdm.sHtML


<!-- 参考信息 -->