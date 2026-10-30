代发 wailian999

[B09] break 与 continue
来源：http://wap.fanxiaobao.xyz/Article/details/gvapdrfhh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gyflzhwfv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqaypnoa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcweigoik.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxogjrgaf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvnottorn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqatwjoq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fanxiaobao.xyz/Article/details/gwkvkullv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdbjeaoe.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gwchgyyzl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrwfgawe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gldcxbmll.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gerwbndxr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/guarikfjt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylonctmu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsjnzoup.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fanxiaobao.xyz/Article/details/ghkzxgnid.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fanxiaobao.xyz/Article/details/gdzikpmet.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/gsixnjflj.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgvmsdfv.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkezdooq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnarlmgm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlfadlin.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gblchmeov.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fanxiaobao.xyz/Article/details/gadtgyeft.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gbgqwnoay.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gbybioipu.sHtML

[B12] 跳出多层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gwuwnrbvj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/gpshkjwje.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvujdlzuk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gzxkdrpus.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gzdhircam.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnrdwzzj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmsszhsu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/ggofmmrbw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpckybte.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexijgogj.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fanxiaobao.xyz/Article/details/gecdbfvyu.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gufqluhue.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrtgkwzs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjphqjjxl.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcoufbax.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqxykmre.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspdhcgsf.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gzchzqvxo.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvwrokfv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihmrykzo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrgyleeq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/ggzzomwst.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gkevrotis.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyfvcmzw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gidbjecoz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gziwfetey.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gwrjsaoqf.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/gomjfyltp.sHtML

Py:   a and b or not c
来源：http://blog.fanxiaobao.xyz/Article/details/gedcyefxf.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fanxiaobao.xyz/Article/details/gsftzslpz.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqstejaeb.sHtML

TS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpqauhnh.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyaucqzh.sHtML

Go:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/glhdnudns.sHtML

Ruby: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gmaqmtili.sHtML

C#:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gjiaqhlef.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gkowrpdoi.sHtML

Py:   if not data: return
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnstxmjp.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gisloffmy.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysiwplza.sHtML

TS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gxvtretdc.sHtML

Java: if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxguwapp.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrgkvxcv.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/gcotnctyz.sHtML

C#:   if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gtasrfbhe.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gogoiqshf.sHtML

C. 函数与作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyswqbwn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gadvardmq.sHtML

[C01] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gooijepdg.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzczmgyu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoipiszj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcssgwwai.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gulixmkrm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqemsrqfy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/guskglelh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fanxiaobao.xyz/Article/details/gqokxfujo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gazjwgptt.sHtML

[C02] 默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwbkniws.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtebcvqbg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhrijszk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gardmbwjd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzsiqqid.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiimdjxt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gksgrkltm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqgvzzuk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbqskfyc.sHtML

[C03] 可变参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvgkpslpd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdkkswsu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutvxancs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/guweitboq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwefvnvfx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gbilwoyrl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fanxiaobao.xyz/Article/details/gqpegzdpl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixlfauae.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fanxiaobao.xyz/Article/details/gszpctbai.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gotpurvmu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpwjcpzo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gaijqncsy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gfhfwgfta.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajzmggab.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fanxiaobao.xyz/Article/details/gznffgsbh.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrouilxi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwilowsg.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfpvbnpjd.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/gtesknoeq.sHtML

Py:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpbrznmg.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjyqqhss.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gchiuvypg.sHtML

TS:   return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/gextgejlb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fanxiaobao.xyz/Article/details/gcqpjwkll.sHtML

Go:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gnlrnrtcr.sHtML

Ruby: return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gshpwuqag.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fanxiaobao.xyz/Article/details/glcabvvfx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxfphpfi.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjazjjoy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnvoljam.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayhhdegq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gywfdylof.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzirxnmr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gwvkbxpsm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqrstfki.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gaivrcyug.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fanxiaobao.xyz/Article/details/givdgfulg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrnzjiaj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gseitqftx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fanxiaobao.xyz/Article/details/glbhngbgm.sHtML

TS:   arr.map(String)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdnjefqq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdeffvii.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fanxiaobao.xyz/Article/details/gvzrszogz.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gqonpzeqd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fanxiaobao.xyz/Article/details/glfrlrbts.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gznnhvvlt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpnjtyol.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxzhsqds.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/guoxkfhfw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcuhwtcr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbobpsqkj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/gjfzqjjub.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeriunvf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghjbzwgvi.sHtML

[C09] 递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gehtqduox.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gikaeybvv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjptbdji.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fanxiaobao.xyz/Article/details/gwrquxxkl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gpewntqnt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzfrsint.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fanxiaobao.xyz/Article/details/gajvfhcss.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gohnzedsq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gifjbmstk.sHtML

[C10] 变量作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gztzyokmb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fanxiaobao.xyz/Article/details/gpfxqohtp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fanxiaobao.xyz/Article/details/gaqjaiwne.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwrxqzxu.sHtML

TS:   同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdnasqkv.sHtML

Java: 方法内为块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gbqexlshf.sHtML

Go:   花括号块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gpnqnbisa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fanxiaobao.xyz/Article/details/gpbmejpvp.sHtML

C#:   块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gmmhmywnx.sHtML

[C11] 模块导入与导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiclwuoe.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gictjkzjp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpuuezqu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gmidrunry.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlbqhmlj.sHtML

Java: import java.util.List;
来源：http://baike.fanxiaobao.xyz/Article/details/gbdicboju.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqtwwdlo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fanxiaobao.xyz/Article/details/gntzivewv.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcvencow.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/gncgnbajl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwymrsvq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fanxiaobao.xyz/Article/details/guflqckft.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gsotzcyka.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyelkmbvh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fanxiaobao.xyz/Article/details/gzjuahvrn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/gapzaqalu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfymnrqm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqrwldub.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdyxkzak.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gbfjpptws.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gawcytpoc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fanxiaobao.xyz/Article/details/gebxoijuh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucrvhjbo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpvjkukb.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkgawrff.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fanxiaobao.xyz/Article/details/gpputihjn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeymrfim.sHtML

[C14] 泛型函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmreradkx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fanxiaobao.xyz/Article/details/guvensfbf.sHtML

PHP:  // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gedmdnfts.sHtML

JS:   // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmczfvcu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiwpkvtd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjgohtmuu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fanxiaobao.xyz/Article/details/giahkowyh.sHtML

Ruby: # 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gqpcifrvv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fanxiaobao.xyz/Article/details/gztfnubdd.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fanxiaobao.xyz/Article/details/gwdswadkp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsxrwyfk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtsossxc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gejrqwfez.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtzavencw.sHtML

Java: // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukkfjnqm.sHtML

Go:   // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjklyhbu.sHtML

Ruby: a, b = pair
来源：http://wap.fanxiaobao.xyz/Article/details/gcinypehj.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fanxiaobao.xyz/Article/details/gxgxpuoya.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsyzagjf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fanxiaobao.xyz/Article/details/goymgvifc.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhabpmrj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/goergtkcl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtzyaunm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gevwwixsx.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fanxiaobao.xyz/Article/details/gedzcayod.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fanxiaobao.xyz/Article/details/gxhhzwyjy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghamywwao.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gaopjdlfp.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyxjrdap.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeeswkqk.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/grpwqidyh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fanxiaobao.xyz/Article/details/gtyfqrfci.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/ghbmkozcm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gfeyfpyup.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdtulspa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fanxiaobao.xyz/Article/details/gpapvufhc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/grgycifoj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gksyitasi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/gptinwghw.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnwnkhwq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fanxiaobao.xyz/Article/details/gpyczdjjf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gtadsngdt.sHtML

JS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzdlvvoj.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gkqkytjke.sHtML

Java: list.add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gsnngsefw.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvouifkwi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnkdtblw.sHtML

C#:   list.Add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gyocacpto.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgmogspp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxusyhyq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbahidbo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fanxiaobao.xyz/Article/details/gdtsketgo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guolbvdov.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnnmpzii.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsufaucb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/gsezseevk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzslxspu.sHtML

[D04] 删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/grksyofbv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmjbtbjh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbjjhydp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fanxiaobao.xyz/Article/details/gpxnopxvk.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofjrxcfb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gggoomynr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fanxiaobao.xyz/Article/details/glpfhnxzi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqeikxvm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fanxiaobao.xyz/Article/details/glhejsxnq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgrbtrcj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gnlgsuksz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gidypjqmt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gtwlpzqae.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fanxiaobao.xyz/Article/details/gcpsipujo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fanxiaobao.xyz/Article/details/gviaraylz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gmmnobrjj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfsqzwjn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnzidkhm.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfzqdkpg.sHtML

Py:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwqdytwl.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjoydowb.sHtML

JS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/ghzptdfbh.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvlxgjkc.sHtML

Java: list.size();
来源：http://baike.fanxiaobao.xyz/Article/details/gveenyjxg.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gbfjsimuv.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfufcufk.sHtML

C#:   list.Count;
来源：http://3g.fanxiaobao.xyz/Article/details/gtdwvzktx.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fanxiaobao.xyz/Article/details/govhchtpn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fanxiaobao.xyz/Article/details/gbnaejfdm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpocghyam.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhlxzvcz.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gghstdfmg.sHtML

Java: list.subList(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghswpghtp.sHtML

Go:   arr[1:4]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvavkugew.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gwikhdtpn.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/goklehocr.sHtML

[D08] 合并两个数组
来源：http://3g.fanxiaobao.xyz/Article/details/gsogjreey.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmscxcaib.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fanxiaobao.xyz/Article/details/gbfbzyklu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzoretln.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvtxnehd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzazigvo.sHtML

Go:   append(a, b...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvofbamo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtlxxqyu.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gohwfunvh.sHtML

[D09] 排序（升序）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwebcgzlt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsxlkbli.sHtML

PHP:  sort($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpyfprgd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfynxknf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoqtwbtj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmmxqwwf.sHtML


<!-- 参考信息 -->