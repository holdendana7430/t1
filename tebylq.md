代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rtyhaaug.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2custqnkb.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2juykvjac.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cbbsufvc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2zqctmyfy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zatyemht.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhymkafq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2luyeauhh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zkgjrhfb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2utztbgdx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hqrstbsq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dqpdeseb.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2shpgafol.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uetzawsn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2iobjbrvt.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jjqxcddk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2oerpyarc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2akpnxmql.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wwxkobht.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xpotlsku.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2alhhwfzh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2afjohnnt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uuefwvdk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2hlzbimrz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gpayivwf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xmmfmmae.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2yytcpctq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bfjqrkmw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2baefwlav.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mbvknzgh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dpxjksvm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xfvzyyhi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2zhfjvyqo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvjzpmyx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2dyowufnd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2adpeamun.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mshesatp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2npimuozb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2drplukds.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vbnfwntm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ckgaxofj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yhkfswab.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2lkjtvcok.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bcikvteu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fmtissqy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2wybtnqge.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rjrgvaco.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2timzjgfc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lujlsvlm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2odbrsdcd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2cqaaynkf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ortppvpu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2neqzlsvy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2xbxazziw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyrmbyhd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jkigughw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jrokqsuo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2risdomzq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2uouycpoq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mcgeahky.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2vobsgcpn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2vfpoiget.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2nxxemnva.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2fbduemgy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2weexaoxf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2likywlxy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ughxakfh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2rifargom.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzcblipk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwyvymyz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2bbwtczkb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mcdqujnh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2cgbzcczt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ewcbowph.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gqicdylb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pitszebb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hiovgbrl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eoowcgrs.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hpmiqsjb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2zmibdrad.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2biejqngx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxglhhur.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2egfjcjxf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wlalbtlh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mpybyhdo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fdwtqqym.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2vkgdtgkw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gvufqqrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2seetvcof.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2iyjokhkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkanedob.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jcwugzjh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hzuawppq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2llxvsjzk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xouewxjw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gblomuyo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gziyuiks.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zabxrsdr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2kvfonqdy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbwgvtkf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xwyvqhgm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2twegmvvb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knjhwoif.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ibriycbd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nlmzeizy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ppavcltt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xkejdaci.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2jmuwmzug.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mzvirfmn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bjqdfbch.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2yoxjtpkt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pgftcgta.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rqwasktw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kbmcklxu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwtnpfrt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2savhebqy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mntwvxzw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2zlvzmxzq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2utwflein.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fouflxxv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2fzbhjmsf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dmrnakva.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cvqdamzg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ylrpnycx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2cwwhbcus.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xfiasdss.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2shmzkhfo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2uhripzgw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lqynryyr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2qbrdvavj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2msksmsqq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2roetglwd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2suwbfqsm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nlttvznn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2phefgbja.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2nxtuxxbq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2bgtqyuki.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2axvueqfd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hgcgctxi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2madwzaen.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2juzbffet.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cewgvuyp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yesrnvbq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2romfuswr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lzgzljho.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2csvcjlqa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2twpsahog.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wtehwwpk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2fuctspja.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vnrlcvox.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ayxczuis.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2sjwdorwx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2nanjpanc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uxqovhgl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2eobfvvde.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hykqiehc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttwcasuz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kbtcjdpl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivfsidbo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2paypirnz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2opbzgwwc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hmjbecen.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2thadmtln.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2mhmgvdin.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2imfnlwsq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lnycjdjj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lsuggqpr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fjbfdlbq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xftahawa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gulmtetl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2exkkrzpi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kfgbadrd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2helxsrzc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2uucezxhl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2bgimdbcg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kgklxwez.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2uvbgvqey.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nbunwgxc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fbiwetyo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2obkfrtoe.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lqqxxequ.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2fdpogjlv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qvzekvez.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2fimbkyzt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2oisopmlm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jdkruxso.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2avuihemx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rrunfrja.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zaysglae.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ulzrqfyv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2atgppabb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2iuvokaub.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2whwgxkcc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2btzryzlc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2otwcqfoq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2khxgcwks.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zqjkunnm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cuvgemdq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2huehmdvz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2bxucjoux.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ysimtobz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnurqtjn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2edusghau.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tzaqxzxx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhlmogdj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rxdtvkyi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qworvskc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2skwhqisv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nyhszdkj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nnabpxxe.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uxxrhrjc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qddlyepd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahrkokne.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2enlnvwye.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2cvtxopmo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2btpwdahv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2sepszwsk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zzhiuxpn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ogiaxwiw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qoxtnrrv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqzfarfa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytqvopqm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2spgmnxpa.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uoumqzzm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hfiuefkw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ugkmasoz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xfntwebl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ythmvqqo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2kaqxmipx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dkbinjoi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fnlcoxap.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txlvjsen.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jqgfplsz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qpeluyht.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2inghxawo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtgpwfyy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ujcvwzrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcrikarv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ajfkmjob.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2isaucjtq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rxlhntdr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mslrjjky.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rcimmanp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2oawrrcem.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ekggjzgr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2sxprlqof.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jhdldiub.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dgqixlyn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2yhtqwgjm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vhovwrhg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2anmkprgm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iogknktk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2cqdxpjgy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2sewyrmgf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2izsjwbaa.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nepoeusl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ritpndft.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zktazcmu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2puyglxqj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2nxtfmmrn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2drkxqlec.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xsxtrqfu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2oklicqmh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2sbqaglyi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2urvdwwoq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pdqcgfgz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zzeeeiqf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jpkifgsi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2wuvzsbmq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mbagwhwg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jpjkwqkh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2glfmkogj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogupxerx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2petaaqoq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bgydlmrt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mlybcqlf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fuiwuoec.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gqxtbpzz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2lhumbwkq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2grdyhrfk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wcnyhfhd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nenfdymi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vxyfktuk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jxnffvtl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2snvjults.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aamekupg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2klpclpnt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mvtkorkb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2tjkfkbfj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rtzztdrj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gsdyvyot.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dhncxxzu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2vkijwlbv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zicpnbbp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mradyoiy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2puaiijdu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kptgctfs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2snmkdwwo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lnfpyyse.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qwpeuuvc.html


<!-- 参考信息 -->