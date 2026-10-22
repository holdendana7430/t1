代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wppesrfd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bhobtqvr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gxsyujlr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2onkduvms.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ntrddoyu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lkeupbaa.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2tvsuzcht.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2coajjulz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cwfplmbm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fireahsm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2psbnwykv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofcomtyr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhtxrfwi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ocoflmwk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2llgcmcbf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2miulykku.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nnfjbyli.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cgesnqai.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2zpzjuefs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnpehxut.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2myeglrri.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jlxkfkgc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwvubiiv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tvmlldiu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2uptzjsxi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nwysifwv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ryvnyinn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pkpneuna.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2girufvpb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ibmthbmx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kptedjet.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nxtcvmfa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2axfrwkcc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ebuvnpph.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ovhjgcmx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2juugqjfn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dfbrpfrr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kcqlxhjt.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qzxldyqr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mwnmywsw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dwqwrynq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ivkszhkj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2yeiubpwr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ajkqicqg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hbkltugc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2myxnmwdi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbuowzty.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mdvujbnw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bhizugnh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2mbjyzgcu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tciicwde.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2erebooyx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2zgpulotd.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2gicadaiy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fpgzahkv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ofpudyyz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sdxnyjfu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xinjfdeo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nmwpszvv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujhkttbo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xkjhemfy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ychdqhrc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2qdrwzlnd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2axfnfndh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2azeqswmj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2knksxwey.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aqvzfxoe.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ljsnhmoc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bpubtnzn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wjxixqbw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uxzciyyy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2noausyte.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ldrkcgvs.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2sihybduw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pwarnyaa.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ykqhuqvb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ssnwpiwf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yawaxldw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kymejdjx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mkdsinzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bejmfovb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ljryovkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsnkdroe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ghkpizui.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2thwoxqpd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fritipox.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bzxxxggr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpmzwvic.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fekovfdf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jdwhnnsv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2zfuyttsb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zljgrbut.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2msbleskh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qxmjrjnc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjuaenbg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kmrclxay.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hteanhkl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ikaeyxzc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ktkaznfp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2mtukqmbf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rdseswqe.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2efmijlvk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gqhwjpyp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wlxumkcl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcisscpa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccrimavc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gesvwnmk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2yipqofrn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2yuibxmlg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ravptuly.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxrqdjfg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2harrzshh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tvymxzxl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2popculwu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2pvrxxftw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zhjwtkqz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2atqqebjo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yyavozmo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwbteoyj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2eghdhrnt.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mthjrwfl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zwoqaqzh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ngsrjkdi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lthfgljr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ucnwempy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qfyhtmnx.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jykioogj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2nntlbskx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gshjghrh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gufdlons.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pldsjwzk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2utacxvdf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cuxkhqwe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jnybzlbq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ckojcwuv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wbibghxj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2axncobwa.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ohzjnfei.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ncjyobbw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbywcwwe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2tskhgepr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2opuvayab.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tasbmddl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2hnrwgdkp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2sjetcmvv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hhaykkwx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bovyjyxi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2aayluddc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xenryswy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2neiihlvb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2luzhplmn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2rhlnxvss.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tkkmnasy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2nmxqgisy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2otwdvlum.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xboklxah.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkxobqmk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wpdymtdk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pppgfvta.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zlssgkzn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2weuwftmk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lvcjnrqx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2abbtrfbj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nryqxcmf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hwmpcqho.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rfophaph.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jmbudpbo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jeusvult.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bflprrcd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jymkmmeo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nxjdwkmq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cevcqbix.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ajhsrbcp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2sxycaqbr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2bdjzaqtr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2kfofxmkz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ztgpabir.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2pxxpgwwv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2kfpbboty.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lopgkxba.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vrptqjuj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hpwrtqyf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kcycvusi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2aizklqcv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ubxqbwqk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lrfvyoxp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ohqvieds.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gdpuvhdo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2focshphq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xgprutcz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vzgwfywl.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wsgfqxac.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uxbcmpte.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbgpsfqt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zckyqzpg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fsvtyuif.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rfchqgzx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lhrzkaxy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2klukhjpd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2siykpdpj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhnnbqcm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2tvognnaj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iddkcxjw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kovrqmfz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmtzzqky.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2guqhzieg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zhwkkrac.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2quhrchqr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hksqfiny.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kdczsuur.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2fxrtyrxd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2trnakndh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktjhwtib.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2anmvwlkb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vdsadorw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ptxvdhva.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2otmidfhk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mknsysbg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2storyooj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zewowkup.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2oxfjvfrr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jtqgwsrj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fixvzzdb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zavafyoy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vqqetfwh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ovncszxt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkdsufgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxskbwbr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ajjkblbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwhgwonn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nadhlvik.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2sctnebrq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bvcrsbco.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zcgwjvbi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zebpwbmu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ylcfrcvi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nfqmfppi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jlpyyztp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rvodazfv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fhbqsgpy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2kvdylubs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2kdcixafi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cipcbuyu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rrlefbsd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2mlurlhii.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dlongpgg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dkfwngja.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2blgmjqvg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tnrdofyg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bmasvuwb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2auatmgqv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ewbojulv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2szxrwafq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xdatjueq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ryvyxqjn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nywncltu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nghaaalq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2yfwkayvu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qeqxhxdh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yftwgpln.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ilokidny.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2koepybbp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kmijoooo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2uddryfxn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xgcfcocv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bgnvyylt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ivbhyewe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ojfkvhnq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xkieaahz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xksoyksj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tldyhaqk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tugkoeih.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nmzuhqxs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sswplmwj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eetvnfwl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kcmgpbkt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eknrvhdc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lxhruxvc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yfjbyxzr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2abrgvzmx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rwurxhcr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xfjmbiez.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vvgjqzmm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2cgpihizk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ivdvamxr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rexlglrx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2burddxdn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2myefztji.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ybwccspg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2noztjhcr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ijhortdp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rvuccprg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mtibtadk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2knvoasor.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yqxtsavf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wnpanttm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ursiqztt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2yqphtkwl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xlyaaerk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ajgukavt.html


<!-- 参考信息 -->