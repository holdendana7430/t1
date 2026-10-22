代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2gxwtigke.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2giodfjop.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nwcjgsxf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2berujfpc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2nxypjenc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzpgxreo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qzssvlok.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmcunyjn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qjocsqcz.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2njagdfrp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbujzkip.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zpbqhbap.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2chrhlbwz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mcbodjch.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2opjrgkmi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bgqyhccu.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jdikwvxo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2eioopdcs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2fsygicbf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cniwqzdy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ciamqjvk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vmbdoriw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyetvxba.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aanfzzgn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qvjcsysd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqoejumi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vxijicch.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2oomikqxv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qzmppqag.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2wmugzxxp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fulcxaqb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2piknxpqo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pirzesfy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wdxvrqlm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyzuwqmn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bzzpotas.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dctykncz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2qrhmufhr.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wymtprvq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pdsmhphl.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ufgvgyde.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2iocesjcd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2feithtqj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ssmttjba.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2wbjjsdmu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zroskrum.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ysngqkal.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2imyqicyr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2howfzrte.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hcfivozc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ogaihjki.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gdyjfsnn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ixroweld.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wdhzwpcl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2juuykgto.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nbldzmdg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2nxttwxbr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zbutlkay.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkleuofx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybputist.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwoofdod.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mpkishep.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2wersqxqt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qeffowow.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2xnuyrbrs.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2uvvwklks.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2iesotvuh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2pnqgucde.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lvyzjqtt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rjaxaafh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ftjlbygd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lpvygdel.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2leuejjpr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gfgqacva.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2dpgjjuej.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jtlmupud.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jyzwdxhd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ldfzwndk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2viwufglw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cttwvztn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oryknfmc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uqekghut.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nmdvozkl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2soeceuql.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vzqyahox.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2yefycouo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cpjrfuuq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2anplplzr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2esndjjfa.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wdfjivov.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vptmrmdp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dyojvjxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gplzawnm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xsmyksgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldoerlhd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cblenesi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lpzggyjs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2usxoocbh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pmlkcwns.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaqwazwp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmcdzvag.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rfsdbkpy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzacshrr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dczqjaqj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vyjzzrrl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2oniwefys.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nsdsnktc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vnejwvkg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nxsvwnpg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2twkjbzmm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jqcyqzpd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ffajufet.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hdsinurt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2cmsywohd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2adqogqpy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2nfridbul.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jbfqfrfv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tasoapwa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2odjsskbg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2chyiraed.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tznjquhu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2yvbhsysy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jyzohvhy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tggmxikg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2uehsbvos.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rneqxwqg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dymzipea.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2aoigaqbs.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2makinjir.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tssllpyk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvwuatls.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2royksgyx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fysljvnw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fssbpumq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2svbkppjv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kjheymfk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2vngpqvmr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pybztjew.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2easiggdu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kebhkfto.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2tbbvegsc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2sockpbkl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2pfnluonb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gppmiuwx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mkjvpdrc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ajswxoim.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2cogmwglm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mckvksur.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eraeewbt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2oepotjve.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2yvaqfbwo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eoysortz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rydmpiqt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vgxjqqwd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nmxzaoag.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ueydpuga.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2eojczclt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2lspolwvu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2imnayjes.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wrkviwnf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uovkqpvw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nsakxywg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2noomaefr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2evnozyup.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ohbvzxps.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2fbbedbnl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yqvbcqho.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hpipjlge.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nqvkfqrb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jiedcwow.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uviodixj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ndificms.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mmzdmjft.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dtcrlcge.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nopliprh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2utodiuvy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2segxjrfq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2juwaqlth.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2htswldyu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fwkwazsm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2tmhunuzm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rhjjsavp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kqtflcqk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2emrnytxq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jyfrlqbe.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2eqskvsbn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ysochhaw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2yqfwutnd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jyudfggp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vmdyzaup.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2mfgmqvvj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xhsobvft.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qysdekdu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pdspudgv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ocebxasg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wiiamqdg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ymgiixzi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wvfeywyw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xcwaybuc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vdqrnmkj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fyhafebu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2nwhdsyxd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mktmpuyi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2lqmpilna.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tsfqbngi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rkwggwjw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ggzliuzl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qwpouiua.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dgcfqnsy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2eovsbtfo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wzwaoctu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xsrayawd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcmshjzr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2avtwhhds.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2guesmonl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wvspmtzm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2qhqfhxub.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbqxzozi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2agtpnzrx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sopmjasy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zukqjcmf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kxsrygnz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ckqktgdp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2anokqtti.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gyoxopby.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2amhdgdug.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rxvnsain.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qvzplndw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2cklvcmog.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zpqamdho.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ebfkthcy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vxqqcvju.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nmnmyhpr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vivahisp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2tkfqoriz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aetenhii.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2veidejuv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2phihkxiy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jldmkvjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajlivihd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jnyjkkob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjcyyoxl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hhjxamkt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vivrpzsn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gjquuaeq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2livwdgzw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2snwlvzwk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nxnwwqye.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rxcjjlbc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eawsbewk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2rsoddmwd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dzjlruhd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rdfzqeul.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tjchecky.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dhxiukyn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2epjghvii.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lliadrdp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2odeblwek.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vcjcvozk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mqheiuvb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yhqomqus.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xschwyws.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lnksbeqs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2xlwvabof.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zlugclkj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ntlldoeg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fgmjbvyi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qvxahxvc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xzpbuomd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2amjpjvcq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2yiitjkhp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lnnunxat.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qjxtnzrc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lqblcqpz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iwothvlb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2usayavji.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2updnjjad.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jmnbhgyu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xcwfkgmq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nzeftapq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eodltemy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dmjgwdcn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2umducpgu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2oockhebf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mkyclecg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ojsdxrew.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jqdamaaj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2acecwlrf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hkgflihw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kbnlhnqm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qqnvtmkc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vffafzzp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lumqwsgq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iuobrbtv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nytkbpxp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2swdxdeqy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2vprfouog.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hsjkwvjm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2obluratu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fncobfiq.html


<!-- 参考信息 -->