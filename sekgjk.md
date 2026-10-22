代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssbcjhej.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pyqzhioy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yzzanbmv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmmkdsed.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hfyfgkds.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jnpkpgtj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uagsngkp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mivlgkrm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2iidhglnb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uywntcpa.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ytkatoge.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gijbidur.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iorhxfjn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2illxzayy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hxkmqgew.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fthqpurs.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zqhfxstl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hvvvsjyu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtbfeuft.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uutzmoys.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wknsyzsh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlwofywi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kiojhdoe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pxnhccmc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jbiltfas.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2oqqudimi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bqpxoali.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eydobxag.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vfemqueh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lblewndn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bkevhbqp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wvvjlqtq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2dzlcazbr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dwtozkfd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2leamitmb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2fetxodpr.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dlkwfxiz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kreconyo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pedzdvwb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2imujdqvz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gcnvvhfv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2wjhnphjk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2rrnikqej.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2pnvyfojr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2lytsokkz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2myhfvhca.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qdtvqwgc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hyegemka.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jhokcmqg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2lrjywpnx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gstefeok.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2erclimkt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ovjggkhm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2gxinyhij.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkkzyyyy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ecoinlod.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nptwkmmd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gypeapsy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ajoercuy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2arjlqsyo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2wrvpyjzv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wzjibuhj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2gderyajc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ydwkssht.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jemyrbsq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgilewzc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iimjfjlw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihwjdezy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eowylxpl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ufhoitqm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2fnrvlsdl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vchzifxv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vtuuwase.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2egmjphvd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zbnupwtm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bcmtthiy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dmpoxnyh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jdlmzzxw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mzsihpeh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2yizrxbam.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ztxxrktk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2atehqkgl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ilhbdoqi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gzvpdltd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2iwyvdnag.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ocfddrpc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2tktzzhfz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wdyxwnpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwspflri.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2idyjehhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mimrdwfk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fbgobdsm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ankttkba.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wptcodms.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2awinphhi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zteyeaid.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zuuolnbg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gtsxboub.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljrqrvzq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gpwcxxav.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2szddyxqp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qauagdrh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwpfgmjd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ndkqfzen.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbjexfkd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2iinilqpa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tuozbehl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jitkpuko.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2alvobdxe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jpuiiwkj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2gmqbksif.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dqbbetiy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mstthwqb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qmfpnvax.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2vdimgwlv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2jocoezhi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tiwjmfur.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vubdoenq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2obrorydm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tpldvflu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gpjyjxek.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzznanfu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hvpveiwa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2okseaqbw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2nbxojdlm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2exkofhia.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pnusztzi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wllrfdzo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2btmlgoql.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kvaxiyau.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2srvjtohs.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2epdjmcqd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zwggnrgc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ksylctre.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zyoiloha.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zffmkvlu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2mqknzwrd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2upaetlnc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2btpbaelm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cztbhcrq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hodcbyxt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2insmhuid.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2fxkckctb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mtszfybs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2utxdorjp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pgyvtkud.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hyckcqhs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hmevqnqd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2oakclmao.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qgddibae.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ohfudbza.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kplnwwhv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2oswcptkw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dijjfpbg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rrvkajws.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gkzstcqe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxbbnygj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwkxxsdk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zubdmqal.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ipvtjwfq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xysirztt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ozvwgsbc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pjsdjfar.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2rbubylay.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2glxltekg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ssqrtdtz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rtsvgckv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dxovkuey.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsmvqdmb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2msbdujry.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ccwnvwtx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2epdyitej.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qjqifnzv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qrnieoma.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2lslaupek.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nvzjjruc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iwbwudmq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xbgzpbpl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wvuofaln.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kfncbfky.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rmgmhxkn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nfwaxmxf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2cfvegmzc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2lrqtkawt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2smpdckju.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wdyjzoqb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2whalikud.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xuhtppgu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rtzrkqge.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2cbnxmvrl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2yxvprgul.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lqejojrv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2snazsmob.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bvazlshp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sduhnoyr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2pwthsvgs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2uqdpzjcd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jzrwuqia.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dedotqhm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2morcbntq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2yrwpakzf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bklkmchr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pqdumpef.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocurvnwm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2axfjpdgf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xawfwxhm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vdvcyzsi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2agzvjaze.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zbaschbc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qqdxrfkz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ujczgvei.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uzwfbtrw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2osflzsmv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yftnzqyb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2bmvbtliz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ajymdbiy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2oslzcwdr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2hxvtzqjf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2sazgytzv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fcsqsksd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xklekquj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ccioseqd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kbpnlzsw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qnplmtjz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gqlfllwi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ucxlbufk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lrilcono.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uviwwgnq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zvptwnbw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2sldabbdw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vjbgkwid.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kzmqzfmm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jhbaignr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tlqtsewu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2besvmxpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lutunzid.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ksqlfwyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imvybyol.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qxebgxiq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ppgucaop.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2upsrntav.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fxflrvvf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2orhgqabm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xtxcwrbc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xugudqjr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tjhvrpbm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vvkijtvc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hcykgmgm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fkqmzsys.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ppceluho.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ynfkpijj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bepouwel.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2yxydmuxr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jbhlqnfn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zatmkcja.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rwjkasjn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2wqtpaeiq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2eokuuyle.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rrzadtyu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2meahsoob.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ekpcxrbp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xrpzzaon.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gydfasie.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ctaipmxf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2olaaurcq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ozsuotcr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ptxecvrn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxlbfncu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2iiknpexa.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cvxdktdr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ssfmhvbo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ipshpedm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dwzmmevu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mozimocq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2kqrwitir.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wkuiwyql.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bljkndbw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2helzytjh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zdjlosig.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2eumgxdek.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ebkdylcr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2puhcovde.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lhncupcb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yruaemwh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mypwkmnd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qiofqwqv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wedqekss.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2urjnhakh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2tlfnshhl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zkjsrqgs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vneermim.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2aabhyepq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pifejkqr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kdeqtrcz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dexauxxj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fjskehlw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2umaqsiib.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kbvonsdc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xebfudmv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cojhpvjv.html


<!-- 参考信息 -->