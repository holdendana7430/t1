代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/grgzfckrr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/gufoiiadt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gavwcitju.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gmhtxvikp.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gpyckmwnu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gnlihamkq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gmxvxbtuq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gwxkcnwge.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gzlvxckbn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gywiprbbc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gbfztiipn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gclrfpgyb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbdaiqrt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gzdjshvpv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gjkhuxvev.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fehbvm.com/Article/details/goqtlxtuu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gbjjsgtvo.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gvqtwlngd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/grgjogbaz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.hesvh.cn/Article/details/gauytrflv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gfbhosilb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gsrzdkzeg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/ghoimxjvr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gjkxzlccc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/ggjnuvsxc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gumpdmgro.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gmdcvxexq.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/gpwarhlqg.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gehgfxzpv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gwyntbzxj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gvoqhddtk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gnnvncdlz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/ghlfyztbx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gsjoxwdxr.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gbwaviucw.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/ghbisaweb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gmbdnqomv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gtnshppgv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gnhrphjwc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gtsyjhidf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gudtjrxdt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gdphnpzuk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gshrepwpk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gbxbefsdt.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gxdrgmxvy.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gustkbkls.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/glutxejyi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gvpgoxhfe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gutgrkkrt.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/giycumljp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gobmhzkqv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gasvqzrns.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/genffbmcl.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gcbmgajfi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gyminkkcc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/grxyrdljs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/glqkkrdkg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gbfqplkdz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gdfqmqjjm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gzdteadua.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/guxzafejj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gvzqrlqrw.sHtML

[B15] 布尔运算与取反
来源：http://mobile.fehbvm.com/Article/details/giyiouxru.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gjrywrxgp.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gxtdiuzko.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gfwmkhpff.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gbrkgvznt.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/graafkjhw.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gdquyvjze.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gtskuhxnz.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gmrdpbtsc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gorbvpbmd.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gxofltmof.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gudgeorwk.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gsivuggdt.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gwkxhovjx.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gqgyiokmw.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gozqjmseu.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/grvsfwzxz.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gwhmqpetv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guldfzrbv.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gulurkree.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gipdhiapf.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gqxytriwf.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/ggopttbhe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/ghlmnvlim.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gnkpvziak.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gluodngqj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gbbjucghi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gmyfjakcv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gcthwgwvm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gndoztoyx.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gidylfzst.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/giigmuzwc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxpomnhoy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gyqhidjhs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/ggjztsdvf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gungedyou.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gsnttxxlj.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gqbqzjeiy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gdiocucpr.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gijagvrzb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gvpzdfogw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gixmyynce.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gflaqhalx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gmctylsyz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gqabcaqsf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/ghepkszyo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/ghtjwwmtw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gqkvwrdcm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/goemswtjx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/glbxhuoir.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/galxselzw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gxnewjwnn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gziwakwmc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/ghziretoa.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/grhczkgal.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/glerotbho.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gkufjhpbi.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gucnuurej.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gepavngey.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gzifvhelu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/glklhtfvw.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gdhqdxeai.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gabydtzjw.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/guuurggdl.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/grtkkyjsc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gpeygqojb.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gxhxjtsse.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gdwnyuvpg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gvzokkedj.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gxmshjwms.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gobfmkkww.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gnmfveipi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/glukbclhx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gcfjydhux.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gmrebmyls.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gyucbnwwm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gyleahfpj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gbstrhfde.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gsudkbang.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/grlctgcbr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gcuidpopn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/galxryaig.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gfvrtxztj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gmokzyzkm.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/ghlqkllzd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/ghfbagjti.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gjkbjivog.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/ggldxyzhd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gqjtepqun.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gwgwmyrss.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gpmvrrwni.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gqdixbrnk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/glzegisqm.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gnycklebv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gusmglzvc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gsbmtyqqu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gxcwmnjjw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gelkpstlm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/ggdkesvvf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/ghbazprif.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gbxypedjp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gnalqqvcp.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gamuygwxj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gvkcoanqh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gypvekstm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gshxkxdrd.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gholmhvxj.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gbqveelij.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqugcldit.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gipiynvpl.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/glnzxzzoy.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gsriuxqxs.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gcrzxbqeo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/grajeugsi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gjuydbemd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gmpvdmban.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/goqufcrhm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gbbwbaakw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gwydelive.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/godijyrsu.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/ghesqrzun.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gkvfbjcde.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/ggmxreqxx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gtamnhemx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gbpkslkpg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/galqondyv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/ghpcapzoi.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gjzjewjxp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gwwsngyvl.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/guybbareg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gvockaoqk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/ghoqwjnwk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/giseqebvj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/ggvytmqev.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gayujqeab.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/ggnvpengq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gwmhpfiba.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/ghpvyappo.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gbzvxthxm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/giwdfoaje.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/ginwtgznu.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gsqijqsxc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gjnnylyjr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gxvyxmqol.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gkgelwpuz.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gmmlcvmhr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/goujumqqx.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gfihhhlvi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/ggxvwixvk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gwggmelds.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gkwopnyth.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gwizngogn.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gidflrugh.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gdixfaagd.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gwvpkkmzr.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/giyravbgz.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gieeqkbzw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gjkyribww.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gsejwbfzt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gyzpqxsnt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gwgtdjowv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/genhugeat.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gvhrgvtmw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gzsbhrgpi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvhnuakec.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvxaavtlb.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/goiuxzhzc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmhrzwtzh.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gwqubuhft.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gkfvdxtcv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gvvjqginb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gyzpashoz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gtsdfhpsh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/guabybidj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gzetqohjj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gwlwzwvon.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gizqoyqmn.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gxihcxlzv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gbsrojixu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/guwxtglgu.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/glwepreoq.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gasfvyjja.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqesnocnq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/giraozvbf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gorghjdko.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gwxialyuf.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gakfqfwwc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcdxyjmyy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gxqcfykbb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gxilfcnmd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gnlgasxjb.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gqcqxdbph.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gitoywsee.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gxixarsyy.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gopfvwibo.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/ggujntiog.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gfbhxlljw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/grtatmnzc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gbssohagv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gjfibvdtc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gffsctkfe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gbnkxbhdo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gonlbsrvl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gukgdmvge.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gtodjeeby.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gdddrsxhx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gzoewfrug.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gktcfkcgr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gvwadaggs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gwddmobhr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gltvgqgcu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gxollnhmi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gtlucslwc.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gwmwkkfgk.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gkmdyijkw.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gyupzvnxo.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gryetegef.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/ghkvljpsw.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/glkqpqbfe.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gebasrmuj.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/ggsjdsghv.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gmumcreed.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gxlisjtaq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gfsqvazyz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/glzktkufy.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gxnnvtkxu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gjocrzoza.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gvwetvdyn.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gdrcixqwu.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/grjcmsifa.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gklkitzox.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gneiryfmc.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gnjgpkbuf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gsittmwgn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/glmanprhk.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/ghwhaowct.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmanjfgfy.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/grdsriitc.sHtML


<!-- 参考信息 -->