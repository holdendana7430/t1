代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jjuquczx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3csnparqs.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bmrcgbdk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mvgupbje.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3evqizsur.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jvndnfhd.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vbrqsljz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vudouamz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3slqwznld.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3iapvfcoe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrlkdwha.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcuxomnh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jfrcenuo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aujlqhwd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zmdydfna.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ctdlrwpi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3awhxlnux.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3vfjwrjuo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3umtsgrcp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnodfrao.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3prpmovbm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wnqqoxcp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxrllwus.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3chudwzpk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dtvfwmxt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjwnppuo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3jjbzbnzn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ncmqcpcn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3itywokjs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qxzgihfv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gddsstsi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wnrzhwog.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hydmuxyf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kmbmhvyc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eajadsoo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lbbicbcj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rwhbkoft.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3iblreint.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bpqxrfmx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hsatdsmm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zbzglbww.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vicuprhv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3lubrpgfq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3yzqieyhj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3dmjycdjx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3pzclhgzm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3vzjbeteg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vzpxnhsy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ntsehess.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ljoawipc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xrjxuhjb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3mckplfjw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jofsohkn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bngtvmdg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vutlbywg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3vvugouyc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3skewcvcn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zrvlioen.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nmjjjxly.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xdpilojn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hkwejmem.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vudoqgza.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3agqwopmg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pemdrdso.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3acpvnylt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gqigxtxa.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tmjhiwco.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jyjtdcdg.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wnldfvlf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3optjyufz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xffcymkc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3djonvjtv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ffzgbimw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pswqvzfb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qussdpia.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xhdjvlmt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zdrebztz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3trpwrkyo.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3bkmgnsht.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kyhsrvqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cholpdda.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rmbzmphx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exqbuzox.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gzaxppaw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ligtllii.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wtlvcgue.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3spmbrkgl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3evcepjqk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wfdvvgyd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lvjicuzk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gxqanydw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3runbryke.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3evigqwuh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3pubksary.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pybpfnox.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bukurixj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gsxwsfch.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3oglgxpko.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3eqgprlnl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mkmrtwes.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ggvbzejk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3duhozeyw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bjavfskg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3pubyvhts.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjhnzvjb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqrpoxqi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tmsfjbpr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3jjujtjmn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ujfbylwy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3yrehbjwg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3thgdjxwq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3inilrwcd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3onzqtjqi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mbxlvrhf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nblmeksv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3boxymfbj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fxkcmpwe.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tckrvvsl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lcufpeeb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3fxutopyq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dfapghbd.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bjqlgqdz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3quumtgsf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jrgtzxdb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ragzjwyp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dahlibpj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ggwepixn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gcmwpovc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lcysmzwt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rpiarrxe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vuapgpbq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mubpxywd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hbpahyvc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3klquhxjk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3dtsgaqrk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xgtjduvt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dclnjiva.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hijxvnbj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbghdpm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bsemolpi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3mwthdckl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ocsflbzw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kxgghrrr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3cutkkxiq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ruddcdeq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3daojxwzk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3yuvsopxl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3iltfyhvx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gpwtcdfc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3voepechp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulbxjhty.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hfqiysmi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lqxoavag.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ipdtrxpa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rchmbeqm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gbdjdfwa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qpcdhzta.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhkgrmmj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hhfwwpnz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kzhcyoup.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtbgtmhr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3cpioezqo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljoaxkhy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3tifyhyfm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gwzvcxtr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qgiznjxw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3zzjpjbnk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hncuhyaw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tyovceem.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wevxykyn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pyudfuwz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3fhxxfzgm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gsnsrstj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ujakcgud.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3aezyofmx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hpjjkuns.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lkuhjumj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3aphezgkf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3yxmjoliq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dhytcctz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xrddvvtz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qgmxrrun.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3dlyykbmk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dqohcwyj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kxbqjexy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hafxcxfl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ifcatexx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ctmbbibp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vdivlges.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3aydlngfm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gorelmhl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oqyellwg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eilveekm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3brauoxei.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wepdsbnz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3upzzyjfv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3unbuowmb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3klsauofj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3iznczenx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qqpkqqpb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3rsvdjgdr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zlkvwnsd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gsovbdui.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3drgpprfw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3brhprrac.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xgodczxl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3arzvfgra.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3apbvwqfq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bnjklmfc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xlyadgzz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3asozjcib.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tkwunxwe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtpovhum.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3mcjifgfn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wvrrzldp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3podpswmw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3scxlhueo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mfncvbzq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mdqadorw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hlidpvka.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vyuhuite.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lzqlxwkd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vvsfzebi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bogtbtii.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fgzfhbnk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3coxaafsu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3lcrsanvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xizbtiis.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ixlmqmsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtcwnvjm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wmfqaofo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tamcyvoj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ywzwwhbw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ygrvjpij.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kyenyeja.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zmzbtwlk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3drxduyre.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iztsjeog.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pnglyexg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3asmoyxme.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3kofzapbr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vhofddfr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wnqidclp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ekwoebud.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nhuprxud.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3squzgylo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ttpybiau.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fdvkbbcy.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dqhnmayi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pmvqxkib.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3giqthyfy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fwunjqie.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bqdzjmon.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kisncgcf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3joizbiyj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnlfeab.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lyyfxjko.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kzwbfvrw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ewzttlpm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zjqjcdcl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3cvedbhgb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ilyzxpyr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zxeqjdtp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3oevrqltm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xyidgsxr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pzrysrya.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rfhlafmi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rdslewpc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mggzlrxw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nhqtsgku.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ojrxhjhk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3exebqmqe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mkqpbumm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qjgfhwph.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pxtwbjdu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ritazaln.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3urhmfytx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eitmlnxa.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3oqheqnoq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ozrzrdzk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zgeylrju.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oaacuhvu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3lswlnvdp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3trxiajay.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mzmcsaww.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dbvmfhdi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ggoofxal.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qkwlzqeu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iahtcmwm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zwpxmtth.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3aaybphwq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xwqjikzh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jbvwvfwg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kjmveylk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mtqarczs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fabddwgw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ibszbnsy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3njxtjzyr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3uxqaxrnm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dprxefek.html


<!-- 参考信息 -->