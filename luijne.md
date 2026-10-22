代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kvczwven.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxqnunm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ttuoqtdk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2aiofjzzd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2udmydwto.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2enpkyefm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2chrinpjr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dgbovghg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kwwydtxy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2tgrjuxdh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqmlohed.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2xmiliszh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2iofcjebd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wzivoxks.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nwfugazt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2otkcnevf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wvdivbgx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qtokbtnw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ibjcyzgx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ivgqvfnd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2nlsxbwdd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2eurxhikm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yglaamsi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2slwletdd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2opkgtptm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hxvackvm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xrxszxjb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2wodjjuij.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2efpcmene.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mgqriqxi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vbjjqsvw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cgqudveo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bmpbavoh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dnthpahl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2pidwhwcq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2syfpctim.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2usmbzzru.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2looouqon.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2llpsskqj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2kgxbrwjh.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wrsvfbzz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bumpbdgt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zkevfpaz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2juwvresc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hpflnqxl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2qhpfqiee.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2agclrksh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ncntowpp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2voqtzbek.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2aicvrazv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2exppzcft.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xaguwrig.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vqlrkyhq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2refscxlk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2eouqiyin.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2tpxytlbg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jymqrxjb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2gicuesrj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vmqcnrbw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpcvhxfk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2khnsrhro.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2eipszlhy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2grslajhu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ggrbnuyk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bzmhovpt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xkhbfoef.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2crsvbcvo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2viosdbpx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ymcfqhgs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2crgqsbzz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nwswyguy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ckelmkif.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eusxhous.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bvmlcphp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vhqpmfuq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2qcjuvozp.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2bhnnvvqo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mscojcgo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2visjxpqz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ooxilvyj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oogdfvre.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ucbwewly.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zdvuaeyt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mlzavzlf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mdmxsieo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2drtkgria.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rkfetndd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mpmqeyer.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pccxknqb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fxgrwmiv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ebgvrmdf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ogloionv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gysufitw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ncljkzym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dblhfukj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2osanrsme.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2csvxtrhx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2typoihsm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lwslofay.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gozfqbul.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pcxbdlmh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wmtxsdjn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2uniiszgg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2omeoctiu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2teikypyh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ogpgevui.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybpfixuo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bpvakkii.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uirewpaz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2hodfxmra.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xtpxvnkf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zizjpyei.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2baikasek.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tfhknzmq.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ynaowlud.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mhvkjbpd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ygmmojaa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mdmmjzmz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyhouuvv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mwgbhisw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kxnfiuso.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2zpyvrujd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2asvfkhcg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rifeseed.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2zxsoxjcw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ozenbkxf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hcedpldg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mzbaqbwj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kyestgqf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jktqsyyc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2widwsavi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zkafvaqg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wxdknysa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2gnyhbwpy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ouasvlbj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ymzfrqdb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kwnuyteo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2asbxjfjc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2seybhxrk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ntjanhcr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2sjjudmhb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xzkedpbt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2kanskjgv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2acgmoavl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bcqwayln.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jxlwmund.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2drsnvwyz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yjmrvxsx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2axhdlgmt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rpnnolel.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2eljzyqkv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vrvbmjnw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2sqpokfcj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2xflzlnpn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xnbyeqlq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2jlupngdq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uwfvmxoj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2tkncurzo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2exlqstlk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tvfrivnm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmygpqyf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jsicxxel.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mopuimtt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cmnpnnyp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2svhsrokl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2byogqxwi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntdmflwy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2badsoxhz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2znatdyoa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2iewhbdck.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ureqwnlh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qnulrcxv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwabalsj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2lonexzrb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhafasvm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2auoasefe.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2jnrnvnep.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ccdhnqxk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2uemizmxz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gilaaeqd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pjbnbobv.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zkrwjkiu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qbolkhji.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2drwtmkbw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zzvdrwjb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2kqtnqame.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2tqbytsyw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2thpvpuvk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ecixlsay.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2glxqzcpe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jfmwemyv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kynfynhy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bkoqvtkh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bnwnbomt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jftgyffc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2wmhaetqd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ojgwenle.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tjdyrhlr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gefuafbv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2knxbidhl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zmoaeylt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2yvcuywqw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ovmfzbrg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2socfigos.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mpltlgvz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmnblhxj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2iolqdcqf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fsreouza.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdaozirw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2sogsdpxl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wryxxfuk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xcpeysbp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvhvrydu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2oasguvoe.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pjsznkma.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nwpfozrd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mxqycjdd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2swjzbrwh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2amciljdk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2atynkicz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dapfbrhr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2omuhjgeh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qukdfqxq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2xtcjlczl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyftmssk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbhwcxqg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mdpcffcp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2frysilfa.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2lyxjcmgd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xpnnwtqr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wchydgir.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xomczjro.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2gbtninjy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2olcmpbzb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tivclhgg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ddziyuny.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2koknbsif.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hsillmwx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pbgwuntj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtczsnit.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2sxkzewit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qaklqmps.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uxwogium.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2knkqanby.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lvbrfpxg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uwmqibee.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2owskwvbj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2pgropmlv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fozqraai.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2sshgodbm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rjlnesad.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2axqhyjyi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2glpvkqhd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nkuofbin.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iyotxyxm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vmqoxlqy.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bgrnngnp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rqhwufkn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqaiypm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bwaxzlgu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2oocrcvvb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2otgotlcg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2myokrsdw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wbhqxxji.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2phqmhozv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zluvprec.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rhkohtjp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2yegdseld.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nbgzobby.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2lpfewxpu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zstkdvze.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2plqrrldw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2eoigmelh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2swhzdbor.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2baoxfegx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kdrpyykp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ujnzrvdj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qrkohxhh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2emuisewl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tfejjkei.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yoctmlcc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aesobxla.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2cluxxpvo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2kzpnagjk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fjqwydsx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lwziquts.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ttpljhif.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pjdrssug.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stvixisc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2onrnseoh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jgqjldtg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2egrtedam.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wupkasnq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cszjjyhg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hkreztqh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2aqmjktpn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hjtlesbp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fahgmkvo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xttoatjy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dvwdnevz.html


<!-- 参考信息 -->