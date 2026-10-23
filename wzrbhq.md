代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3knosocmr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fgbozilu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tcvexywp.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nalebduv.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mveddzbc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kdzmqwaz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fpvufpyq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ujhvjpbo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3fheqbgvg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3qygosfey.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yejfhztw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vybxaxwy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uvwaqvrk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgyhnrtq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mrsnxqdr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3totvlhcv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ismakeoc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gqbbjhbd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3idzyrjec.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuacykri.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3koncqkjb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yngbwxaf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3tryrxppr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gbbirelr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hvsebyom.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmlfowmy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3fsphjyuo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3oosvyffo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3wqwfvmti.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zowrvgzw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3txlwdcia.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dmtyzskm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3lnrydofb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vupfhzfd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3etdkypoc.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3krggbhjm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wsebyiad.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3gcbhnhwy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uihxpwfs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vqvnczez.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vswtdljy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3clhmbhcy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3wcdkuyud.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jokldmzs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xmmdtfzv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ipgxtyfn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3noxjxpqt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bsmydcmo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ohxfmtfj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xgurzihl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3bhjkvxja.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3cxtzfhen.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cdbcuvph.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3efhbrfxv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tkzlihfu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3gijchvat.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iqjayjmo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzwrgowt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zazqocaq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3epakakia.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lipuxvkp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3txwqbybf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3hnwoayiw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3gjlycxeo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3iqywwobb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nltmcwex.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3teyetzrw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ejtuirmf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ajzuezjt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eavlkoiw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ulwxvtlm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xxljfufg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rkmnvipz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlcigzsp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3shpangse.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ivsvqtjs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zgmpofib.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ypqjmiqe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hdsomlxq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mzkekmtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyuqlhkm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jyniwqry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsosdaqk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wyqojter.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hqkyzbqq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dwnukqfh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdkxctyf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qppgsadd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lqkgosyp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qnutdiys.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wcafgtdq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bmwmcgky.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tefxyjtu.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gkrhubch.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbnomusz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxnyjvgm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3asllvfjc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3dhytivxf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3eimnhhwd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mkgqjpxu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3arhyzmqv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bgfvqupf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3yfevvvol.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bojtrtlv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xecyzdop.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxsvpbcv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbasakjv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xatqcche.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zigmqhfh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3uaowdlxe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3blmlrfif.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdmrnmh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3pkhdwpep.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xarayupa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3folezvif.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3itbgluzy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xfgyyddc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3upzvesvv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynlxfcxx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dxblxfqp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3savrunwu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3vuzmxgty.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zdgruovg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dexpllmb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bkvapkxs.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ceepvfit.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3teozriqu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qjkwbxss.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jgdxinto.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3orgjtprt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cbabhssa.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mdrarbqe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3khuyoayj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iiiikzuo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3yufvsnpf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jjkplfyp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3esebfnmz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3xgxypsym.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3cqduwtet.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ilpxhipy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3rapvqeoc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3egrsllwz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmzsbzvn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3sgvsegpl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fnbgpuch.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3thmpfblb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vejpidft.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wutotuqo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3dqnvjyzv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbofmfdl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ziaffqbp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gjvxtskq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ntphgovw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nvgigzbc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jvdrvmbl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ljtafpit.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlxbranz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wvbutigq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xntjanys.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3osxlfkjf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvvublpo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kechhnfv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zkcvsrna.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3alsjfjbt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3iibqskog.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uoyxrwze.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3uikhewhm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aysewzxt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3iioorapq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nngrxyri.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3txkkcgob.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3azrosigg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rmhmztke.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ffbesdsh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pjrpxotk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3eodoqqcv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3adjuegck.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hxheteqx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3xcjpghlj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3suslemzq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ktygcamy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ivgogeai.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3faiabrxf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3izttnhic.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gegctsyx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wpvbkslh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rqtsxaqg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zamvdavh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3rkmtgxys.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3npstajwk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vmqjetyf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ieendqag.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jnvhvaiw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xjhlcnug.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3uminizhl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ckosssci.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3azvoxkrq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gkwtcwkz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3iaenyypd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lldjyxhj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fobwtjva.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3mofvkgri.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rijwvoib.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dzpwnhgc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zpzmnwyf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vcrywafb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dzabcslx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fukshrfv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3tliekkii.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ajfmhlwe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wmuxlaus.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jfqaktyr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bryvqubz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dypyrkhc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3beblgixf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cpyjfzxu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jtskzhjw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yzixvjmf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3pzuyrvsz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3teyalcsy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3uvlavjiq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3uzzjaxmn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3fikrlkgl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ozuqpipl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3cwlxxvzo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bxfjsacq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xmiufglc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vomotwmm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pvwbuqfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkdkgmfy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mfsfglqk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jeoxjxwv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xiunlchs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3goyedagd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ireamzku.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qmxnyhqg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3burzakyg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tmvrtmmi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3etscfjth.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kfwltgpg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vjcezyyv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3htouyymv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lqylutkp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fcqmbinz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ebyjjlfy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ebdiqoav.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ugxxcnti.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vksoxedf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3yuhpvyxq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ievlhqwi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3pagxagjk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fvqaschj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ytkwzhkw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jwjpdifa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfkfyzb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3muayjuec.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rlmenkgu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3vqpvcfti.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oftfqpmv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fixcwtug.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3fongdrwl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qeimnlwm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zinnqhsl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3enipjlpo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yukathwd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3tlgxtbnn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3oskmljsv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3seqcoprp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ndgydtvv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bqsgyofu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3exivmlsp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3majofzlw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xsprqkdl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uxnfjeii.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dnuyoggm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3avffkwoy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sofcgcyy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gzsplvcf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cbyjnyzy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yzeyesom.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3khfcmxdr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zvztnwsi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rhexaqjm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3tytdbyza.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3fbohxyzm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3anvuxycr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3krsuourc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3stiedtoi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zcemuxig.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3anvxsfpw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gqpnzfkt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3qhygxevd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rceticge.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lsdvtzja.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gtbuvvru.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jzsyhqjf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3vbssnqiy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3omzantes.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3devxxsfg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uaslvpud.html


<!-- 参考信息 -->