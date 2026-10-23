代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kifjutjo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hwxufdmi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hpvwqatk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3utjiqvvd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dmycfarm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hriptpet.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3btowysmb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gshizdmk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3smchoqnd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ukxwpthv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jntwcgon.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ghrxihml.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpbdqkmc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwcqhgrh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3euigrlul.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3seeneclk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ipbwxeku.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3sdcckhlu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3yissatba.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ohvkfhin.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kbrpazyi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sixeetmb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ddrkxfwg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3orhjzdja.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3xnfqfgtg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tizurxar.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ddbfdsed.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3afdumqef.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3eoiizibn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3slwsasvq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bvysinam.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lojnqvvt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3omeshuik.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ffgtbiyw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3thpmfnkj.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ekbwpylv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3reggqbqi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3qtrlylgo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fzbpaxxk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nyugwnds.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bquxaukb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jbxyvczg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3plnvmecu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3thkppcqw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vjhdnnrc.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3fnbrghyy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3vxxtfaml.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jlvqsdyy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3amheosfh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3aterhyay.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3flqgzvqs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3gexaegdc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fxocpzti.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kxurnvig.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3rqggckuk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3utocnhyy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3anjluuzs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxqfzkjn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3stgmmtas.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ncidqgbm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uftzuxlu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqpazsx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ghmbdief.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ipcdkvru.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ihzajaas.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3amjiwjid.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wieqdlzn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iqwwhjnf.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3egywntww.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ixijhigd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pmylcxut.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3mprphzxj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wnmczciq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3udarwfly.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3drdtzfrd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ehtnphhg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3twrwmmdl.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xfcxvtvh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3jdaitzhu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3szhgvoxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjqqppzv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3mgrvwwot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxdmhfvl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uhenhwhl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zdncfcpa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3psjygedg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rltpqfcg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3urajabaa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xybkazlb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3knsaxzaq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3xmgpejxi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaedeupf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3bbjmhath.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3rzaeqvdl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxtffnph.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zkdbcxte.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3stffzmyb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3hjnueffq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dppdivnf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yqclipvl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3unfxwcsk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmdgjvxy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3avzuowmt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qlfosbzm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bnzsipwt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlpfptsc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eylpqiae.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3dcelkepn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hpywegdf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3rcqcrcql.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3genkxmrk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3agfeawnd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ocrdpreg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldvvndwc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gevqprcv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nhnzafsn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ladxfcvp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ksevkvvw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dlieeqvj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ehnfzoje.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zpirmjdx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3qhcxufsy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wormnhop.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cnbloreo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3dfblvfpg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uygcexvx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fpoqvyys.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zecfgrgc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3uiivufqh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3alyexqeh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ryxkmpjh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qoxztgeh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ldbyswpk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cbztbuex.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3kctntknx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3skuxexyn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ultsyoor.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3zqjwwsgo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hdqdwrhb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kotfglmd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3haisouot.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nbvinchg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3iaxvflnm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ayweuocy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jqnhnxno.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fnrmkvan.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ohbsmxzr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vvqgzuff.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3avwjwjih.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wywzpotd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqptubpv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jniodclz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kdhkjqwf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fezpnhdw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qvkugbqp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxjmjfvi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yskkisnq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtqvvwue.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xhgpkvzg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dkdnqunq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3msgoydnw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dxhylprf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hoxxxsmt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3tvnxwspt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wsbrvgmf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3tfkdaenh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3cmcwdozk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cpcxnnsd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tbnzqmwm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ozrvqgwf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qedjpttn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mmjfnuze.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dnbbavkk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zaszmybv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pyazgfds.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ejhfapro.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qnftxtxv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3irothfup.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dxqumowa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3tmdygfyi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qwbkkpnc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3lugugqxy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pshfcges.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jwftdidj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zqyvdddp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3muyfutqy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uzszdpwj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3sugxetzb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mrzgwelq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3oxmscaer.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lkhtmmpi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3zxzoldrh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xbuhjgjs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dodkjrzz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bosoouyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nuttydsp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sisdeknf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3frhvwdoy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3clllilpv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3oynvhmxf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gdmvfice.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3moibxrav.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ohpqgyje.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pwgekwek.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jsojktqn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lwmcirib.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3znnktlvk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3whueebsj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3cnmisppo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wjnsyjkx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dzjpkuaa.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iulaitdh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jjrrfczy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xmiyktwl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cfqjwdax.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fdshjzul.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3egcudfyi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tqtuwkcd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gppeqsin.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3pghwvmbn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3queqrqhh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3odgimuji.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3kfwhpqaa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3moacqpba.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kivclafg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vranosov.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3katqociy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rlgbxdni.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xedadgke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwvpwznr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xknudivy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jguwlvgo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rmgdybpy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tlvsaips.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ctccapff.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3srciczfy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3gneaqtzi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tvzclmqy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ryjtmmqs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3abgjhelq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ulhhklht.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lujvmbsv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tyrjpees.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qqskznyr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hqfrlkpe.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fqokurko.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3inxijbsk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lyhqnjiw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pgjsgwbc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lreasutx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nbqceeng.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vxbhwldh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wmwreaom.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3arcnaigs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3spduridl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fqizwoju.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ukswdncn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lajdwzja.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3gyyxjqia.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dopcalwv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3yytorkhd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qfzssszv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qeexnyya.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3yrcmmxck.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ipbkqcvs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gamuiwai.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3onopramh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pydhckqx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kooveusz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eljdncsc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gmjrzzif.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fihclxzx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vsawthar.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kuxpbptr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kbqjdsfu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wfosukqb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ayyszvvb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bbmybttf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3povuftwg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gszjoxih.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ervesgpn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3esbtomml.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bjqxmvzo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yesdbqxe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wmtfxbyz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dxjrwcul.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rgzywacz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qwfoywlh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ipnfpsnm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wlzmhpjv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3seyepdjg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rfnhtgra.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ccsvpdmo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3myujfgrc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ahgheqso.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kkbdvill.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dpsrnjsi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zcgxzpvy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zklmmtwm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uemllldd.html


<!-- 参考信息 -->