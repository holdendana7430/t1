代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ebvvzric.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rubaelmv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2brvmyhug.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jmnstwcw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xlkcilbw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ucdotkrc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nhrkziba.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yazzhrtv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sgccrqgg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2praganif.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2qlylytet.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gbtfvdch.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mksmbtlc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ghhssonn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aerqydvi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yykhjhkj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ymwlygza.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkvehush.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2krimjuag.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2bfkxlgde.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eghraeae.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vinylnpd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jstkeejx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2svcxeftk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2icdqklad.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ewbzftzg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zveshoun.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2khhtqeea.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2utrnxwcl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbjyayar.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2nylvispv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ugmxdyge.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2uwqitkap.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lgvrhfjz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2uvhmwxam.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2shcpzuex.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dessajjk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lyjmhvof.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tdkgamih.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uecxkkjc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2uyrbuxps.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2txzmwmrd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hzcblnsd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2muqydren.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kylaomto.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qzibslku.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2oeoxmfqo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mouvnyaq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gzxabtcb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xhjmlukr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkrqtknk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ziqkufcu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vkwcxwqe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2brxjdfll.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2yofnxlic.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2amwjyfmd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ykijtzld.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2cukqmnio.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2hcqncbnj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2fcoxhdld.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qvzxrcki.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dmlwpcat.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ygijslzm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ugabimki.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jyyriwoj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lyrpaqfg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vwikwpmy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dmgimeux.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2akzalndb.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2izeskpse.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uvsygzdb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vlxbyraw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mbqzzmaq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kcehwqob.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jlgqoklz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2wxsvcotv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2enhxelqe.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2phyiphfx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fnyztzzh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2imuguira.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xsfhbpwy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2futcaecd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vynesmei.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dwgwpizw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2buaggcpb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jbxlvojr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebdvcixk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dzoofysy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2pcmlzzde.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vlrzhimo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2efxqigoz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qdgopcrf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqehmzdl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2daszpgkl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ksjpdjhe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cdcubmxu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqutbmvr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2iriitygb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpchlyri.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfkvqxuc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvxwctuu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ghnsucik.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2mgqlrwds.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2soyijyzw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2sbshkvpt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2roehtbzi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2tkhvywld.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sjwbpxus.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkzzrbwh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvkucazi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzdzfmqh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rtgxartm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xyfiqbzq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jtjxbrnt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2vjmsqvqj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yxqcjapk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cntwwmze.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttbibsyw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yycjeezx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rkbpyurx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pplaparz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oygxjyjv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lksjaxbs.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2mbuyzsqx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bhadfort.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wqdthvfi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wxegdunh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2tdewbctl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ywruzvhq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vqkcvvgl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2axwvrxgt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fhdyoxxs.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qesrrtmk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2uzaolmaj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fefooznv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wjoqukwd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2czphpmzz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ffvocvrg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2reqfkmeh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nxavfrpb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ugmndcer.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2oesiblcf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2emguywhu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mbyfsenu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mytcijii.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2bgpxsgss.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2gyefcsks.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2paqcwhvj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vltitmti.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2kfjetdul.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2vdgxylho.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2unactwwz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oosoiiww.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2inhfkwlp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eergsnuh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vrvlfexq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2udtyvvrf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fbjnvxuj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouulrdyx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jtlmherg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dfdezlmf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucaahxwq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pcmaqwno.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2aipvsalt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cnmvoszf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ptujxxnq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ahejltok.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hwxyhhiu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cqygtkok.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mgxxkepe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wufmjxdx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2njihstdv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2eckokjil.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oiqqqpfl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tuafrjpb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fdngwzdb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gfdpyajs.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2anmusyqe.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qwxvwbby.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gsmkhnss.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2iphhpxeu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2efykcsmr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2oqwbokjc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lfzpzpfy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2aolovdwb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rnwhiyvn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2sznxpory.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2nrknrpuj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2luugfvdq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xhhsuhma.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ahfeqohp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2glbkozsl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xpcpmsqi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cdehwgka.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ourgthhv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qlxxwesk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2broxbdoy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fushnwdv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2jvoufeeu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kriuukcc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcvthkvb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2haaudalu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zsnnjlli.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2fifimwyo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ugkgfopd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dgnjaosx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vqsaddtp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hinhmult.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2slutyaxs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2tidmhngm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2znsyuvqb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sdldvpam.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2exhnnxni.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ewwbfyoq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qwegoztb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2koteedzs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hfpbysiu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jrjozsfi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qlhdzhlp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2plybnzjm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2iffuimfm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gxgbizal.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fxsykzlm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nbsxvgee.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mntbomdx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2llrqdqdt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2gezxxvgh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2iaubxpoz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2nlsmyuwy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lqkepinc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2noyvyhas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufcxqsyx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zxmzhjst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acvcozgf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cwhccaiu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2pzuhmrly.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gqozhtpn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rzbtjiog.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2anjnwihy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2acpdywbp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2nrgyqtri.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2iwwegjdj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ddzeeogv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lsdnrndn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lqlxxxux.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2npvqigvg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sykilwfn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cpgrzixj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bfxuiyiv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mexwqvds.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2effsqjhd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ecvsozla.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2cmqxcmmr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2stiihoxn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2iwthgttm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2patjmeep.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2chmtypft.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nzriflfc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2roewggtr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2uknlmelg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tpmjenkj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ibnqaxnu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2hnrafulz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2eruhpexy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2avllxiqg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qfdivuhs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2daqmggqc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sepkwdsy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2maaewgkv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ebwjkrpk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2itisufbt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sqywfdnc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cohxsjwk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kqaixxxz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nfytezuv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rrvvpboi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bqlrkdqq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ydbzowns.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2htvwujnt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pcjqxfim.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgkptyuu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pvpisfld.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2valdbpnd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2iacgsusu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2pgfbaegy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rmalpmrt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2dwkvolrk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2rmrbejwr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ivkquclx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xdigretd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pvpizagz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cyvecfml.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xbtxnwzy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zgptndmc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2juthpghn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yzhsifrw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2akoumywx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vdmymfbh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ldsekscb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2igdcbdah.html


<!-- 参考信息 -->