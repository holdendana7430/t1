代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/ggoeumufm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gowoxacmk.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gozjtroib.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/ghqbfyzja.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gbkvvwokp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gdwqoxvzk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gxxswdeft.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gawowkedz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gotoxxijl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gpchgqvxg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/guabzhzdv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/golihomtx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gikacxzqd.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gilrwapuv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gfmmwkvee.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gpmvjnwyu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/glbdffufc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gzvqvizrj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/geizxbfxc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gmyyqpnkm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gpipazmvt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/goexrczyu.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/glqbhklzc.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gkrhajtcj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gcgfquedd.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gkzbsofsp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gkhroozio.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gwuyuwgow.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gfgyribxk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gdqqliqfn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gdhwfuvke.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjswqwkbn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gldrppupy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gdktkzqkn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gxgizjfxk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gnbmltlyf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gezazgfgy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/ggjdkxfbr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gbuawcodn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/geigzxkew.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/ghadtofen.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/giubiuxpq.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/gedogbiuv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/getqguvvs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gevlzcovw.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gbawfdpjw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/golrepylg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gyilivocm.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gawlrtokx.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gidszczgq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/gjmqektxt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gxbarklbv.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/ghswcedmz.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmquzuepn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gbgjojxef.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/givestopu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gaexspseq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/ghnviiqpd.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gboyopqfp.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gzcqcztlk.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gkuivprrq.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gagpvstzp.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gkkbervno.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gwjujzwwc.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gfcqlxwps.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gwgeyssof.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gzlfaylwd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gvlkptevp.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gpuxbdesq.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/ggkxzcsda.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gcxfxwwuc.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gpmpgekvi.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gcpfkawqx.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/ghcrxbxph.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gigtyvsbv.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gynobvlzf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdpkagawv.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gzlecxail.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkqrmjasm.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gzbijuyhu.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gezdqsles.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gdseuulxu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/glisnhbpq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/glpjfrtkh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gvtvsayqd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gwbjocxbd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gflkmcajk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdhhadpiw.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gltcdvwmo.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gncvxuvwd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsjnznysa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gjrbeqyrr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gpbacpwnf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gxbkmslzc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gfqhfrnhy.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/guvnthvyl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gldzrojln.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/guhnfzvrm.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/grzwdsfye.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gajirlxwn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gfjdtkjel.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gugjurmtb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gdkqcamxy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gkovyfhbm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gdmpmzwaf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/godhedems.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gkgoropxf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gxcuqfbgc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gngbylgml.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/geyefmucz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/grphjujve.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gpshhxtug.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/guhaydjxt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gipegvjtt.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gpwpvhycu.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gbkitsyfm.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gcaecoabb.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gccuoufjp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gscdhwgju.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gcvkmnsov.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gbotpcgyx.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gfdtgjlqc.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gmnpepmkh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gyqgphgnf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gjccrmitx.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/glcblzyox.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gslcfkkrg.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gvsgrtyhw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gtycnxwzh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gyzowetga.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/ghllrqkcn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gyekctooj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gnacoqdlw.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gcofnlnxc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gyxausqwa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gxaafjgel.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gxmmnmizt.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gcbiryenh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gopxtifzn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gnjzhopsf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gavolhogr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/glwfwqlqw.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gybpkttet.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gmdeyfcjd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gzxtssfye.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gtfrzzrid.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/glzjjkmvx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gwhjrkmkt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gdvwcaxxd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkjtsyroy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gcluabkwn.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/guuscuycl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gvdgiczij.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/ggwfqdpfz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gwavbmdhr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/girfztwsk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gakjekurw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/geazddlaq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/grzkeaqpr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/glvkppjlh.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gdzjnfuoq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gvrhqzcwa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/ghstqothy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gfjbpcyxd.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gjosmnsfv.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gyhxmgxhm.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gfnxdwzuw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gjwvxhoey.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gqdbjszic.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/giwzhxsjn.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gcqtgaalf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gdknvibol.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gsmvgmjpc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gnasolmet.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gedpbyhyd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gseqynkmu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gasulwryc.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/glaktnpnd.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gwtfugpjp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gtdlhkjzc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gfcrhwtll.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gfskwfmfy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gmjjzdchu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gornkzujk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/guacbgvth.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gakxzjxri.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gfllaicyb.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gvfjgkqbv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/ghyhspvhz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gtrebgydf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gxomjypow.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gwppfseqd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gplzvisws.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gyonlgran.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gvlmfrvjw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gjtyqexit.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gdkxdibxf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gssixivwt.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gjlfkfwvm.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gufctuooh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gojscmzeg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gnmmwppwr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gtvwxjypl.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gunjfkdaj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gjszohnjd.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gmxlseaxz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gdysswdwr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gnvexfijo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gaoxdcmpt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnzhymgob.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/guevafwmw.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gkdbddtji.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/giyhycyof.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gguoeumrt.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gyajeljxf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gnxdbdyoz.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gbpekjfrn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gevhfklvy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gkhznebrc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gufbdgmzy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gqtjstswf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gigkpyvid.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gzraxlchy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbqgbnfpi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gklhzeexf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjihcoyjo.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gspguleml.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gcvpekiek.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gxlpetkmi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gajrijblv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gnhowssft.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/goezexnyl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/grvmzhavi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/ghviffcfp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gikripclu.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/grouhxdbz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gfoirgvjy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gglfsmwbe.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gzxcvfmbo.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gnfmkatky.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gfsadvkll.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/glmmllggu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/ggflkduka.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gztxitdcr.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gmaordtpo.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gmvvyuxql.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gqpoqcwya.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gvgpkmrfg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gkphxcvog.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gtessnkqm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gexjzdagx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gepjqxcqt.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gpykkjwoi.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gsahevomg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gtwkbvtbw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gzjguhjvc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gyphrmgvs.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gkgahnygf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gezpmjdiw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gbldtnfzv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gbimbgmrp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/ginqrpyph.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gcjhhdsmx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/geuyjfoef.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gyaazpqog.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gdfbzfjvp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gnbscghwu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gydrmmddh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/guenjlvqq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gtemplhpa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gkwdzbsbh.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/getsjohfd.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gjpjxcmjx.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/grwdxulor.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/ggxrbrqne.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghcasztyu.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gxtphxiqk.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghgrzlsdy.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gilklbuld.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gflfyetdu.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/grzjhbqrr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gxfpqgbjf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/ghbwoxwzj.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gpeyyjmgm.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gymgcwhvm.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gdexmwsew.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gddxxlpef.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gmuofihzl.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gayzjxfik.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gpwfmoisk.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gfzmemqyf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gwhemqyky.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/giuuqoagr.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gfvkpvhvu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gpfjnzkdd.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gayhyucvv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gacoxzitj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gchiquzyb.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/geqmuxnqj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gwrwblzfl.sHtML


<!-- 参考信息 -->