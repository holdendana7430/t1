代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2clflbnqw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifdvrasg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jhxjxanh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hvmxkpko.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tltavjqk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyjahqoh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2njpbjrws.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmmmlmjo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vtwuznts.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2aannncnn.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2joztezaw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2jqquooyr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lsarmzjg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jmdvmpwi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2izgxgkzc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vhdqqmkd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cqxzrdjn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pszohvdm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2enrxvxlq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dpxxktxt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vvfifrgz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zspclibu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjdqscli.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2apotiorq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ympdbayr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqhbqpfz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nqtgjlmr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pwynigez.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2maltliae.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mquwvser.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2qyhhjxry.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tdoreenq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gsxdocev.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fbluhmog.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqwpzuio.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2lvqikeqp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wuwnjeuj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cxxmwihz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2wlnvrbru.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lcaoylqn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pohudcax.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xvfusybg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vbbbtrac.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mtnucknc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hnwsyawy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2hoeyebcy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tdcpiclc.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mdvqxqdu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ycltsxxa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ntjcxrdq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cgfugksi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xsvvdnsz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kslubspw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wgrjfsuc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2fhuxnlaf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2cjbqgrzp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xxptvimu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2devfyfxr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fqqlozow.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2livvylnt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iwrbzana.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2enwkuski.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2sdlulpic.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vjwnfwpo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ujignwpw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mlbafrcf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yickgroz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2mqiczvcp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rdfzkczd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xqljnlqs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zuhlpaxe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvmsqpoe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mfbebrxw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbwcjom.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kkfebnff.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2tdqbnjbh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2excedukr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2grnnrcyi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ugzzwgfx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kaibncec.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zhjafzgm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vtuxquoe.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2krxrzjhc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tsvsckdp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hnxmmaku.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vmgtfaja.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ghzjysiy.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2sucmeyhl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fnvrfkqb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2sfwqdrco.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rsyelbvs.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hqblrnzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoocbdrv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2lakkgfqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smphkiby.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bssztdnj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xxygrdzr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2itnqfboy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kvugydmz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpgjjnpk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2awztbgyj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ypdzqtyh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dqqdjhuf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxklbrdl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wbaqxrpz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2revhblpl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbvwnkqr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgufviyp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gbpanhvm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xlztiqix.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2cnmvgekf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2kcscreon.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2jadzmiby.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2oerjteuc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2wkpfbcpq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzpcctom.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xpgkftil.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2duoyfflt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2vsutbvvq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vcvzugdz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ugwweeuh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2yivwvtrh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kgojanwd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2imqsopfb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ubgnfswt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rzbfsmvj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tepakxjj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xilhwurn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2suwpbrhs.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ehfpngtp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lubnedgm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dsfimqfk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lznusjsi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zkohofjv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vfmpbyvy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2atvesrul.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2eupipbii.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cbllxoqn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2frrjnimo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2eyfpiego.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2oslbaawr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jopwnmzr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hrtzbukb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ogxnragb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zofldmes.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vyuxdxtz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2azryxxzk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2brvmbxsn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ylbmrfqu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dwofydze.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2kwgzazde.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kxxvrdvr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nbtgvpjm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2qakhrsbx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lyacfrzc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2kivcohxd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2swjpahvh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rlcpbwcj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2phehawrt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ztwnbgzj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgcmrwmc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rkewvwev.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jblcihia.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2bsgpyazh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bwfjngsa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2thzqtyyw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhusilwd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ocsvnkrd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ronnsakw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kevttoey.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qjdgjalt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wubbdfqp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwolrhwa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cuotcrbp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2falcxwbm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kcqivirm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fxknhxyp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bfimaawj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2sactnlhc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kelislij.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pcbatwlu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yxesqpfl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yhxnndlx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jrikliud.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yhmrboud.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2kheqoipm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jeqfhaqx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jjxchozy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mqagqpwz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jgxfftbw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2nvatdeif.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2petbnzhe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2bwdnltcl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hintijro.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2hhzedouc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zxmhthki.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2lvjzgnpe.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2szlrjaka.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ivtqtlda.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2eoddmyfv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zensvzpn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ktdgseko.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gsaczwni.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bgxhpluk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2spxmwtir.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2acjliall.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hrvanzbv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhwyabjr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2izchhkkv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vkfsefgz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2pnomltiw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nydmbuoh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2efnlzmfc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2uvuygyng.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kyacybki.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2npvswunv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2teuzwety.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yewaxjuy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ggzrjdkg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rdezsmvx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2htgcvasy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2pnzzzysw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bkljwvao.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xystnwvm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2twzdduan.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2trtcxhpg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2edhiwdfm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ystzenhg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2igmlizrn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2heegtdlb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xdqtqmmi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vyydurud.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nxpqfuap.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2alzkqrjb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2szrfuttl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vnwmznro.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2itfmgqyu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2pdxaagkl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdqbjjeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhyenopm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gmotasqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntezuohz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bylsuviz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2houxspnh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oootqgkz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hqyujwia.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vwytiijw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ntlsoqwu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2bvhotvcj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xpubohqk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cxcezrkd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wudkavtz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xnxagukr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mlbeklpd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2umgrdhpl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lxxowywx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2rsvmbigj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2azcktdjg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tpjoupsz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2stjuwbfd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wlefoilz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dpltqmcn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qbeqhrim.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nmkadrme.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gczlwwmd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kppbxfcx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmqsccb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjzuuex.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nsqphtih.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mtdghler.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xootivfp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bnwssudf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gcjmprwi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qrkllhwh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kacqkiqo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ldtbigdz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dplukbgn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mireltgf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dchkjtgk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aalqirqe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gbtkppok.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zpqqkjjf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wjvdmfvf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ahmidzug.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pvvektqc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2forvqfeu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2egsbkbww.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dmqgxjme.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sjpjqucu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ssmqycgs.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ujcqcfwz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uuruzceo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2cdbhayqs.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2leozasab.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zpjumctl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mqntoxyd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ofmquunv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2yubzmekz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cecoewdb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vedeiubg.html


<!-- 参考信息 -->