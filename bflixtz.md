代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gdvmolhyl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gwmagtyea.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/gmejcmbyl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.hesvh.cn/Article/details/gtrvlrgqe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.hesvh.cn/Article/details/gxehrgnne.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gdggnyzlo.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gewqjdpqy.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gwpydmckf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/ghoycvaza.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gjsxzwmyb.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gmpiupwof.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/grlupdbli.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gpsrlqjcx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/grhtammvr.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/ghamoxhbx.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gxrjenlxp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gqdagaaai.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/ghiegufco.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/ghnpbcwwj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gxjxdypzm.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gnogxcnum.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/ggpsgoqsm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.zdbjq.cn/Article/details/ggktgqbnf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gtarsvosg.sHtML

[B09] break 与 continue
来源：http://www.blog.hesvh.cn/Article/details/gbyibdcgi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/goezovcvf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gavmppqht.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/guyykrnat.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gzbczfnjo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gqwdtdllg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gghyzcdjf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/giwdtwxtk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gkwlrnuod.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gcihxskqm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gtjgsywta.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gmlzpfspi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gvpzwoedv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gnfgomoji.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/glmwljjmh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gdzqvsdyj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gxvpdtyfw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gnlrpxaia.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gqjclxxzn.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gowngibta.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/ghooekqbq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gaxdwloey.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxwftkvkv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gjjzwnuxy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.zdbjq.cn/Article/details/gpgdmpphr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.zdbjq.cn/Article/details/gbtjsteln.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gpmlqzhko.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gmblmlsni.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/ggicmkwhg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gkochnzav.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gnqdgwyrm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gdhhzzpes.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/grdkvchza.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gryvhpnnf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gvbkhtegx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gwwuxydta.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gdptmjfir.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/ggwuxiana.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gsixxdzxa.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gobcjjwhr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gunkimtnu.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gmqoilnxq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gzeegnvca.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gsiupzvxk.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gontoeijm.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gzndqchji.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gbjloqfjp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gebqvuari.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gulqdlkgf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gewyithth.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfzijmsnr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gzwnhhrus.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gpkecpmqf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gmqinbqtu.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gpnsjpdey.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gmqokptba.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gjyskcbxj.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqugcnqoe.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/grexlccso.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gisifgoqb.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gixbpjrmp.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gqenigmhu.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gziqlfzmc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/ggnywqulc.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/ggrurlmyy.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gidntwatm.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gvwcylghn.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gsegxhgkh.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/ghrygjgld.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gkiuepwmd.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gnnuuqikn.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gnqpkedjx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gudvcvdaj.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gcwknfljj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfsotvzyp.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gllfhuuns.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gjxfgnltw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gvbhobtmf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gnktosbbc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjhncthnv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gguxuerdq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gxkzwnpua.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gdiwrnmnj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/grxlwidut.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gzdsoszxd.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gknlgmgza.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gfltkfnsp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/grctklvza.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gnvozylob.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gqgossmii.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gzahtsxpo.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gfxyxynrv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gqlzyhmqf.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/glmvxktfr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/govzzcmvg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gutmewqhv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gbvgnyhqq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gkmmpncea.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gxqeqasam.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gdoauovie.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gwsxwyuub.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gnahibmfk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gdkuowxuk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/ggijoyora.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gvcfgcscf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/glldnjxoq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gkhqqwtdh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/guannlhui.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gdcrwsopj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/grfntofwz.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gurgakome.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gwbyowteu.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gdwyewwic.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gmbvacbuc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gshlsslra.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gfayhwbgh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gtxawgzgr.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gopgmvmgs.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/glgmzlhmm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/giadhfaog.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/godxbusmm.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gnzdfojtg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gdxspummm.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ggutldwbw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gcdxgmkna.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gyvyjalov.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gookfrgkp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gdpfyvaho.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gmlrbmafy.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gsliagtdt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/giualdbew.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gwkfxxjuf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gljlumnjb.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gkkmuuoow.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/guazznbfn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gsbndjlpr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gbyrvaijh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gjnrrajie.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gdafffunc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/ggdxkifru.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gteymrazr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gfgpirnvf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/goigxajiu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gtukftzoo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gnayzapwv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gsbwvwyyi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gvazydfpu.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gyuvvjlrl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gxbsgblqy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/ggpjwlomu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gnxfgqaii.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/grbwywifs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gxnoesqdb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/grtiiqrgc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gpckvsbyq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gmofxbkgn.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gkprainhi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/ganznzdgd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gmisgqfsh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gsbbsatel.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gqyagaifi.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gxnnpdgnl.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/ghxmujdjz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gwkyrvaer.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/ghpslnfvl.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/ghjjwimxq.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gkgodwwby.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gnhzkajgk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gykmfxwmn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gbonherpw.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gnvcvhjpw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gvngxnuyf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gkijeyeyw.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gzlggbbjd.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gvcvhmrkn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gieublzlh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/giccadgvm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/govmnqfit.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gbdyubpxn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gyqfvuocf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/ghphwpznb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/guegrwryu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gtlpqtqaf.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gnmftnjvp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/ghwpbycpw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gyiffcyka.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gqmwhvizs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gjwtostwc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gassuvmof.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gwlomyouo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/ggnugelmo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gnogxaeeb.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gphequcpr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gzdlfdxht.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gwbbvpwli.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gcwwamwbg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gjveuxskm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gmarqluzo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gbzekthpv.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gfjkkdtyy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gqdaqjnoh.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gwsstigui.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gqefeyque.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gmrloatsm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gtuunjlny.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gblxuvbqw.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gtnxgzawb.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gbrkbmcgs.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gkelqlybo.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gvzwlpoap.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gseqadbfd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gnzsuhxds.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gbjvbxvzn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gkmqdowdm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gatwuptfx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdlhbqhkw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gnsdxgcif.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gogieeyfh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/goqkkgoau.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvklcqqoa.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gxjiwqdrh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpxpwgjyg.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gyromgpip.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gqaxpfphy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gchsoxogk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gnwdnosmg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gwbmhaihi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gnzsorwom.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gqerxzzpn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gomjgusms.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gsvghzote.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gumoetjms.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/glwswpfep.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gfoejjjif.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/giayamfay.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gwnrtrnhv.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gtjkllsnm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gpzwqubqf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gdufolmru.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gsztcftpy.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/goexcufhg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gcglghivt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/galbxuuoo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/ghscbooib.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gaxdgcvzx.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gxtafkqvy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gljapseuq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gsvuitsjj.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gvthvcxuc.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gmckbgsmr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gzjutxnla.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/goopgljkv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/ghbbjffic.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gfxmwjyid.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/ghlkifgno.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gwishimee.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gvpzccgwa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gcvydggxj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gwdyyyetd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gboyrbeab.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gtfzhflrv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gvhbbagqu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gmnyraisf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gcxrgibeo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gxzanncho.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/goyycefgd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gpxhcdduf.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/goiefkuxn.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gatcwyebn.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gevptdkrf.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/goultppnf.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gdysrhnot.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gegvafjgj.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkrmgpzrh.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gmbkmwxes.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gzsibtqbz.sHtML


<!-- 参考信息 -->