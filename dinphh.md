代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xdmtgzrk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eyffhjtn.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wqwjngnb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rxdioybg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3skxygytf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gqrxuiah.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qauhbmnd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rifadwxo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rtutauyc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3eafxytkk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xsuczmut.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aurlinga.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vqjqqqyq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzgsuczi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hjsjnnlq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ystkszyd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zdvukxhm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3zeeiiceb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3lhdfhvqx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bfuhrizb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dbyfuxlw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kpafxztv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3aszsbpeh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3phktonyc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3htuenpel.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sakowigi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3czilvpyl.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3qztmxylu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kcjbvdmd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xtvycers.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ulsentyr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3akopcalb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3gxpfpsqm.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rouhemcr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ivaccfzw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3beklseyl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lftavtyy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3nujmhoin.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3exwmoiuc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xfyqvkmt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3mroydkaw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3hhwsjocs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3lvjlqycz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3zojajqrg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ldkxmfhs.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ziuagbdv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3vdnycdls.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwjdegbq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3keuptvxi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gnwrugfa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xjqnhyxd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zvikvbgf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3cmzsysoi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3mdenmkpp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tjbvtsgl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hqzscunu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3inyjsipi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3demanbdg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fynrtpah.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3asipolzm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3njtqcjnu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vdxrgxzb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3yqskhtlf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3uoocdxen.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3zqpapzne.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ngmnjnil.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hhpwbhuz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kejeimzq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gjldxgvg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xjiapalx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bxxqseri.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hgetfjex.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ltvzbhqa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rmpdzjmq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fmurfuij.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kbldiixf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zpojxpub.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3siorgbtn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3wgnwwiov.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cplspjjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlgcmiri.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3erdbedgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npuvhmfo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3aqvbouhd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vlruefxy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vfewxsfn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gnrzsbop.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgsubuxk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssfdaqll.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aasokdwj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3lluftbdp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwdscxfe.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3yzehuhmk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ngnajjqi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgjpyjna.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ydxdevnm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3egxqritv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ujvbuusq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmsbmqqz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3umzwlogc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3emmfimie.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3subtjngt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xvzroaua.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qryldkgo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwaqqbkr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mzjrafkw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvxydhcb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3karvnnou.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3krejadnm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rwkxydvl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxxulngv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fmfbjnyf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3matpuzgq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zddlteby.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tydyeedc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3strmxdjj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3njhinvhr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gafatgii.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qesklkfb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wxicrtyn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3scqdxdku.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lpniazab.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uvixjwkm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gmparykd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3spazurvr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qvyuqscl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3exazbjay.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3obnfqoik.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3otxpsepe.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3skxdoasa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3gquhalvd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qsmksmlb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dsfnsmbh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tvbudwre.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ebpcqfjm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lxkiszfy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zwsqpzbx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3dbymibxm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3gztfigkk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehaxanhe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jhifvifg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvfpycd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3urjtbgnm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3frahasqb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3dhwbwmyb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3krgknhuo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3cptyywvy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3esetjjlp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3lbbxubik.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3efbqflxc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3doazlhky.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wglxkbha.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sbsjezyc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qnjyjubr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mojafino.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fbfknocm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xfhzwzub.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlvertuu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gzndnuor.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tvhbvzyq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgixcilj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3neyzoxnc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cnvolgwx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3evfwrhwe.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3llxbiehk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3qpcfkpvp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3msbzwvuz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sepcmqol.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ediwxtfo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xhoqygzr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rfduxzuv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ypkrxyje.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nljdxora.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zbcplkua.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3nafreluy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ydqgwnfn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ujqggvwx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3aandwafr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3gmevhlgt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3xdcmiuma.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3gtmboqdr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3cmmlklwd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rltxgdtl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3neaxanvr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vmbmwgpl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mfjplxqy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ddmhwxad.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ayjychqa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gunefhru.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3bpxbajdu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kkcsmuaf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3btxsmdxt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3plhfzhky.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpkxlawe.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3fynddbje.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxsyczxc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ieoxwnpt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rdtxkiue.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3cefuiwhb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3neuyoktp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wnxbjtib.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zsjdndkz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bllyqxrn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nyeajxjp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3dmwrquqp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3owyuobcc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ikhcowcy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tszxiemt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3aajyscek.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3oydalklf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dltnapvy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nmzsgfln.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oijeqjfv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyiarafl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qjhsqmuk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kuimjfjy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3sqdnutxu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cxtdvmtl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3klypimbt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lvcluyet.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3nntyiuin.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jyaxrsfe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wwoamzvi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgdwtzag.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3forzompn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hcexyduf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oofvclby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anuukwmb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fdxscqra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hftegkgz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qlucexhc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tddgitjf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mbhvurcg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ihkexeyt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kixciwlh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3yggrwmuu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pbufhyrg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3duacuddo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nlbtqyso.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3netgrgxf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3regoptxx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ctqmyqth.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ycgmffdp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3whahrwos.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gwcpqaci.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3efigczrr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lggetsuk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rxietvff.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wbnhtntm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jrreqhie.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yteufszf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3glgaoxfp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rozqzmfc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nkcsxwbu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3yiyolokd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mqpmcxku.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3obnbhlhf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bxfbiuht.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lxxqzclh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3hpkqxzpw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3finbkhqp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xrgcemnk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cocbqkow.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3cfdninqc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zplhamag.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gukghmet.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wrlsyzhu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ldyqtyvu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kjwpozxo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cqgkmyij.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3krdzumxq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3kjkdqqnu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sfgxkeld.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jwptyrcn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uelsydlg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oqjjkefm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sqlvijcn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pixtcebc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3keninsme.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lfefamaj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oakdedgc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjdawjyi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mveqedsp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3daelqdah.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tvtrinqb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3qsbrqlsi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oocucukg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lsxbebld.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iuhhpzut.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ziuzznqp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nclwdmdk.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3uwgfkaqr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jvjynebb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3prlptcqv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lictxazy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ngxtnzvy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3jogfzfbb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gboyqked.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ardxzccc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3pjhmzmjg.html


<!-- 参考信息 -->