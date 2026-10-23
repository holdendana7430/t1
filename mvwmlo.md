代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3fysithjx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fiwswukx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvevdqqm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3cuxuwpcj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xmycrvls.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nwpspeal.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jsmconqc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mxgfuncc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xmgfcsug.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ngpvlhgn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kkxqqzop.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3haiapeah.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3bpcowfsc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ygmttdsz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3opzmebfc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3aygbyovi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydzndldc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3onikawfh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hoirzmlq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3eigchqeu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oidcxkih.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kfslvwqx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3mxgkvgbx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3lzktnfsk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tdnrrztw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zybvwvok.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xslvpyrx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3mtudygbu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bfyutbzp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gvdlixta.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pcyksgpo.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ilxaeqnb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3almpzpws.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3htiuzexq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3alnorxyo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ymravpnt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3vhcgmqly.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3uyxluzfx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vnkjlhoo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vfojxrcb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3vbfjeeco.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3bzijuytf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yvomyppr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cypdoike.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ulznhvad.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3vcnbzpvm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3himvknjn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gblabgig.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tpxkgnhn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3oqaumkca.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3gnvkjprj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jiptgflp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wmwpupxf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3mbgnzjow.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3xizbwbkg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ntfceugn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3owyztidl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vqzpmdoy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gqhxvqjd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3epghdtgv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vjttuszn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbatyzvv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tovccmsc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pabtvbok.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3isnorafb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iufwztmg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fnfswsjt.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3tecmjhnf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3apbuicyv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jduzpdsf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ekvgevdh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3azlrdfnh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ohwcssln.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kdtoxgti.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nynigccz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3wgtsgbor.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3fgrauefb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpaadeke.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hjejyvui.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uxwnqaiv.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3yrpvqvkx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jjaizyvf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3nczjijfz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3eihcngvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcbpqala.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pfmlggby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsozdajn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3onjtoalv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ilwuafup.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpocvlsr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ntealgax.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqdfyzws.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3znlanksf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3scsmwrvw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3vekkzbao.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ysipcgom.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pmeaxtfw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jrtsrzwr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3csagunyu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctttxfbd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bofoxdcs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vqdupdxl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3brjkfngx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lcopkqxs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ldxtqrnt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gjrfgvvv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3umzegdkb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnhkaipo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnbahctc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jkypmnqg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhoovrvg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3vufyxpbx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ktfzkgah.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xmibvgvz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3aawfmqfb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3awcifqim.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3pwskchnq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbevnyet.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fifqcfex.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3oqwssigv.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ywmivvma.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnnxppxv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqfquehs.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kdoxrcgh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vicwubcp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ljhtyonr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3duvitatp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wgsbvvfu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rljadgcc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ibdgclvk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3japsbiwn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xpqzqbdp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3nafqstsy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3hpypfkmw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zleexzsy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kadcenql.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bcfxaohq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3oykvvgrj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wcewmbhj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jbnavxnc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lrnhylda.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bwyxskdl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wyuuuunx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eexfihji.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfxnhbz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uzajrltj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pwuycflb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3maunduvn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3cyduilif.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jhloffqd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vgqjxazv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ojxfolde.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3pjyyllmj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3njeeeder.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mddniaaz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fxkjlozq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yvfaxeni.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3htawxolt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wctjkgbr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3uolyafns.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vazyfmhv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmvrqgel.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zqfhnnbw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nexivizx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kianpjuf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xzxeinnu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjcnjiyc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3dchasdba.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jypcmjpb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3fjqkvevn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3laswnugx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3yrmkpvup.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ztmybleg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ybhubmyk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jvmqkaqn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3jjrhpuvg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gtwpsuxo.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3onddahzz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3bdahnzkq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lkkqpgiu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nhqxgjgb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vieqqisa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nxscoyuk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mguwzhyj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3whowcrhm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mqbfrqbb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3cslnxhcl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tnkvdowm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lcufhhii.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3acjyysoh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xabcwgdf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3aalqnijm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ikksapoi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3tlvpvzhi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xsiamjmj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3lqwryrse.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bpvwebhj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yzgjbwob.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wzjfxuec.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jefequmy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mnbrazpm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vruawuhf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mipusjlu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3tqejmufe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nnioyprg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jmprjbwv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cukvpdfe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eeaolbuk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgyufyjp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3skjlvfda.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3fyvxdavi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ylxqplua.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bbiozvho.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3atxhiplc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tcxpbhwb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vworygpx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qnfmlddh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3imsmoxlp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qthjwfsc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ustxphab.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3imyzxqja.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mmwldmjl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3uwgjfcwy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nrsggyhb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xbojikny.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ueyninjy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ljtwhstm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3svryjnjy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ntoebuvh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3tnwfkjnr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfxmkedg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xscdshug.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3jjlplbsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atmexvrf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mrnljcav.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3heaaklxv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sfmxctmb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ervwebmq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3txcgopqu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cyvomzey.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cwmbccaf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3stasilis.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lmiamtyg.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rixtwrhk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hpghrtrv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lqyqydqr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vzcuazfb.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cwevswjw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dfxlogkx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gxsxmjyy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3eqwffxuk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mryrrqce.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3shzykaov.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ndqmbtuk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3lozthvze.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3refiddsk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wscjixrv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tiknzbgh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3feqgefpg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pldrppwq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lonceuwh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jpbmpaxw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zpkzsjwr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ysztsuxo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3moqdtrpc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fgwbuaan.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3dpkwfrbg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3saiozycr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cifjojif.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3imrvfclj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3tavnljej.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rwumguck.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qjgskqlq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ccmhcqev.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vdlmitpm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jabbjmax.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aacltsxj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gzyssgby.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3viukbmou.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ilieymni.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fwswjjwh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dtuciize.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3asgjfirj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yzgknhvy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3sxqxazde.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uyozwqon.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pbbyfthk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3tkgaglvc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ecwwwbnc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3moxuwmne.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zijdyvcs.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mpbofgwv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3aosnyboh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oleloaki.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eglxeych.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wyigcmpb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rcujzfdf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mrgrywvx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qoaxoqks.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3gbbjlbvo.html


<!-- 参考信息 -->