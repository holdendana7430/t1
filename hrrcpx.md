代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pnvsqqdv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ytauggbb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gdbyknyr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3jxsupqdo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3kqjsnajl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gvxmfhfk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3iuxcxkwh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kbbmyqrh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jnryoegl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dklwelha.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ihowsfcw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zmtgcbky.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pdcebesz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3nvlqctrh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybmultzn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uxxxqyhd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfsucmzu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdkgwhsu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rosrbqku.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3cmllsvjw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwnwzdhw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jviiinvo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3nediepua.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3cimdhblp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3llsmmhle.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fsghirgq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3abianwux.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jrtfmjqq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3cicmqzyq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3glcwldjz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3sujnspbh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uklmuzpg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3bomzjzfn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3osicfttb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hinbbxtu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aozmftci.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3fscusejg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3whwocmro.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nllfdbbp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3cjvpxrkm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3pfsankgu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3upjkqfnu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sjymfgiz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nrufjljj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ewfhsxgq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jolojigx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3iiushshs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ehlsafev.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xmjtabzj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tftkgyim.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvvefiva.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mncwhxdv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xuomjrhl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3rpufgyxw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tdvclhtc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wdtqdsqr.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3apaofmkk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3brebjbgs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3kpxpznil.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3khhihtvr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3slzkynna.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3unxunmin.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kgzbeykc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jwhfzrzr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fjxloqcz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sprlxava.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qjuvrkiz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pcnblvsl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kuhsaqgr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jszunzsg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kutgorbe.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hzmbovep.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qmwupexq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gyhaenfw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hbsvalbg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dxynnkua.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hevnzoab.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3eongccob.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ayvabkwk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wzgwemna.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hlulecpo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3noxzyvir.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3bzjcljjm.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jfcajqnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynoybzhm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wvrvjtxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qghbyoez.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qzgcvohg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xiibqimw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpzhvzmv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lslfnfwn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbdvyqul.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvchcink.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3innfjzec.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3onwhicpa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsrugkzz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bohcivhk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mbgbkaxu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3hapciivg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ubkkomuo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxhnwqwe.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3evwnqzkk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3sknlqspp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hgtnwqar.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3refdippy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qqquvurm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3iwvgchri.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3brhuoinm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yltryzvd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pbwfqegy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3aoqaouqs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rwoknvxi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3zgkpkfbp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tmjictwb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3tifzlvaj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rekrxlrl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vouijbiq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wswmdeia.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jljrpvgy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wzuddmgu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ompgsxwa.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uucwoymt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3staenwlo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3llxsdots.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3goacmtqi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pupdynda.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iteonhqp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uhrrcmca.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3shcqklyq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3osxeiymw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vgjzsmeq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xppclhgf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3nnisaxxx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3fophvxsp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vnbljuwc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3niwotteg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xiykfhau.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3galmynin.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3adlpuobv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dntzokql.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cjiucpkp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3aglzyjje.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3mcnlzljq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtdmruvx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3llojgmxc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mgmcqgyb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3uewkzaqe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nzpvamdm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qbodecyq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vcbjzwbz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gavbyzds.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zlqswhpr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbzpqbyb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmvwpggy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccyrldlz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ivckcdge.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wcdifgpo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3aknkqxfr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3feqolqrm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3peycuxmk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cujlyssr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzmitgnx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3llkrfvxd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xruzkpuh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbszbahn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zzzponhh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kdpxscxj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iggzwdcy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ffbycuqo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3yvaatsqi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3imbrkupm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3navvcjoz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3akfzlftv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3orxiaacj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wlikinus.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fbohiyzh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xmorfvwd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3keqnstdm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3calmedqx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3fdarlqsi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nbaquiau.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zgpztzaa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3aqixfadg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3pgtgrahn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rlbcvstu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ggrvynuu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3souyudwx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3uxmgnprk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3nrczeyxp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jftpmmsz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ahathvcj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qikuissx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3idkvergm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ehqlkxjr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gpkfepdr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3npvdmdcf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vtepxtng.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3caweoife.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3rkrwmxru.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3inaxefho.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fugnunlj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pnoidosn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ncdepeze.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3brizjfnb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrdxylqb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3orjcjhye.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pyetreyp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bbznremf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3yvbqcnez.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3htttpifx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bbvqeqaa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3azcatklq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3eyshizwu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3yqizhsob.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vyijjbaj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bzyvuphu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqpjuyxa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxukycqx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3iwcislgw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sfeeeddt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jojqiqil.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3llugbowl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vvigvagf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3gnpmtxuq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3lsuncdmy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zpvsqvaf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3btrjzeyd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gkkytgpo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ufhvebzc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3tgmlmbai.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkdaqrmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmotxsxu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3lvdruqdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuvtyohj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bjqsysoe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3izpeawnl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wvynrdfe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wdyozwbj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ggdtpkcr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jdladpby.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3sawijlqz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3faalouhp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ukkejhid.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bsitzvwt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mzrptzyy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gnebezwl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qttjrady.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3waxaujja.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ecjxpbxk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aenvymfv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ovxccrxk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3etfnhefw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ifcechlm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zghlvxzm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zsyvynbj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vinbjgun.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pdwtpqie.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jtxougwr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rckxwywi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ipiylbzn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zwggxckd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kzzmyrnw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ieiltdys.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xaxkwthu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3uafkvxku.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fxanjbma.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xmhwucrl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nqnfesvt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3udscmfqv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwpmahzh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lrbnvmpr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tedphzqi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3awbzenrr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3svijoiec.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ofixxulm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ivrxhlok.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sliwcwzo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kemnxkoi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mpzssdtk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fccgthxh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yeeggctq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rdqhtzoq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ikvgcxcq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3urouruuv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ezajslui.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hvnicjsd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3lqghlshp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3lpocfvrq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ihqtxatn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lzfwjoau.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cnelscuh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lcpazrul.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hnucaewd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oolnzleb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3txssxcxv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3dbnkdfnn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3asxeijos.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qpzervxn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3orsnvkic.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zlgqlmdw.html


<!-- 参考信息 -->