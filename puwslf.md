代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kbhzlsfc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bkkzzsgb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cfbwonyw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qalqqvlj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ufkennfq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nbqjixxl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lbiwzogv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xvzzqgmn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gbkuvgpt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2aycccyjh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vyhjxogt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2duulushd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2imvbwiie.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ehstapuj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2scfdovbz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivzujyop.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2njemjtjb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2onmzsjoz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rasvnxul.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2taycqamx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2secxpzdm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mtzpfjwn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2epqkcyci.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdayafmg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2urlengmc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gmrxnxhx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwoaahmb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vwzwyptk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pkrkqbnq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2itextkqx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jdkbmutk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2tqeclibj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tfatpjce.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ujemfqxf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2orkxcfnk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2osaxucok.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wnzgsetb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zkytulgb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zqoaimve.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cpofmlcn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vzqbigxw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2flxkgtnt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kssgpvke.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rvhxefgw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kqvwaerj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2pbzuhqsi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ejhihssd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2lgnxjjke.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ciajumlk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2vowqlwwl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntyoxfqh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkzrpswl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yukwgvrj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2pmtzoeqt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2qbplmpnn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2odpdlmvs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lqkuzmvy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2kbxrybgl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2emtucnnw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2bgzbmlfq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hravjvaz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2epcvpxes.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyjaravm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yybrtyvy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edlvtvkm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2awjysyzm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nowpdsfn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2uvubooyl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2fdombnog.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2exmpoxbr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ssdaulhj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tmvykbvw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xvjxulqi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ygprgozd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yqalpsgs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dlberxxh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2krvwwbfy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rsmctqzk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2racfdzur.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dmpplkbp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gtpzzktx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jsmsuvea.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nedymbbg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nquyvfey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipcidcrx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2oljkuffj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcdamyal.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dwbrwzto.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2maodynzi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdwqcecf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2afwbiqqe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yqmrmvtj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2winxafrf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nrhgxkcz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dqfvoycm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgctfjun.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2rpoyqeia.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qkxyfzxe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2fauepiva.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jfauzjqh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lweqoaxg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2taohoqyi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2szjndcwd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2fhxshqkt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gmbojery.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ygdkqzjn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2jmicrrwv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjdvfwpi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cefzdkgd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2klwymnln.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xedfwqwn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2pgizmwmc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2pdmmhcgc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jhxzgjpo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2icnykyzc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2esoialyh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2mlnuzllx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohzmwhtt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ejeypqrp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2gvfssznk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nhnqorfi.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ovmiyrfi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tiqabymb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nwkabxhg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yosljrdp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xhcbplvn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2yycjqwyi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zomvszqd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2onihydhf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dwfrrdmd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2seusuuix.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qaqbzkos.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2puuncths.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wnagdmzv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2elcgirud.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vseytyqx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fedlujqy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2bujbtdre.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gyyritcp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wuyoshbs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ntsralsa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2btgtchng.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2objoibqz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vnmjpfhy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2heccfoqy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tnhgfidk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vmmbtxas.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jhyzpfqc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yuubeexo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ukdlocmx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2plwbbhxo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2iejnldin.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ebkhmatt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfjytgno.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwsmyzoo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2sqgzvjxo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ajngklej.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yqejokki.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dbplzuck.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xxrzktzv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2opphrphb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fneidizv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vouqpyvz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2audshlna.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmjdsagu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tkcmysws.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2whlqtbjk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2chhrmiwf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ngaizkbd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jvnuohyd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2oyodoucq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2hucttixo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yyjtremm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pmsxbadv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jaaryufp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ojuqgprd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qentvxbb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lfmjjuxb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2edmhtwnc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2hwngkwba.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2kfokhwwj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gfkkjlby.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bzoujftf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mqvmwffj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ljxufzje.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2eivqxwwv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2dkjwtfxe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2hcaajcim.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2heofciqw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pwbfpdou.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ryyxgvef.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2zcytcyxj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rtrpjmhl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ozsorswk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cotdrvyt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2noyxxjzb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ptyuykbv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ttaurlnv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2heulkyho.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nwhyzmfv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukguxhhv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2etmfnnpv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hwlpaizj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dwhtwjdf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2cjhrvoqk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2bpunqksb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2toaxdfia.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2idweymmm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlqzdlup.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hljsnplv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ealbrtpe.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yhigimfo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2yrqhlilx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2eswxqthx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kwqxqvuc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fwexdljl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thpceqgq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kelbvhkt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jrsqktfu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ftsmanzf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2lvqvprgh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kpvfneek.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2gzjthiuo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2umdfkebn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cyfgabix.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nwyalomd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2szrqrnvz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvobufml.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bmscbcai.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2liaerrey.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2iallqsjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vomhdwug.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pzeeffod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khksdorw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ffqftyui.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fteahxve.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2illrcvqv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2veaidubg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2yjpdvkun.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2zphtgfzq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2umpdehil.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pdxyaxmg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2csuwknzn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xrjhknvc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lnmhmsip.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nhwxlsrr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ccxfhjku.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2opwxnjdt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kouqocbn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dmqjerbf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2wwbkkzfd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jnvfotbd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gkgwmefk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lddlcpql.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ddiohlte.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2fhtmmdqb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bbohdmdj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sdawqwpb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bcrthsuw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bhyfnoro.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2snpgryzj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2cyhthuiw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ltupasht.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lniexnwa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gdxteeon.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yzwnobsb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hunitzyj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wdwdjypt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gwjjehsh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kwgrvwfb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dtwzofox.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cdpxwloz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lvdefsic.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2krlhkkiw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nagdkwfb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jsjmvbqu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2agdroxns.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2azentiuz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oprvpgqn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kltrqjeq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhadgsy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nxfnlkrk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hhdjodmb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nbzyeuvn.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2rljfjfho.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yyocwnga.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2prgrjqdd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2yeciwgxy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2sgioceup.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ysgpmqpn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2shlqbdri.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yfdeqwqo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gzwrrmdx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yuyvhmta.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vpvkrotu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2fmvhkjkt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sglkeulr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wpyoddnc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdpvmvr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2thikjtro.html


<!-- 参考信息 -->