代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwdwidbz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhlsqprh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gntsakxn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sdnnljoh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hcjlaruz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wtiicuga.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcbqczri.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2crfbsmqt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ehcxuccc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xqjmhfld.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kzieuqls.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zfzjafij.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hpiyceqi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cepzlvzt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2epwkpcsh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ocsvqskf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2sogwaazv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2cifvxzkb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntynlpgs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2imzikduv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rtuqjsrq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmcoorzg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2oqxvwhlg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rfyqpeez.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rcylleod.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2oathihsv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2uqsjwcle.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fhaomfvx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2tvfavgni.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xdqpxqid.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2qbrqoeic.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gebkmavb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zgxmwwbt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozjhfgux.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2hqgtgyru.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gysthclu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2btyrtxjk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2srznynpl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tvzsfuky.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybtcdqiq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2znicxhjt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2pvxbzidl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bmerbsxf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rnarigsr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2aobqrwbe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ejwvvldv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vqnqwgax.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nxdlnjjw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uybowhpz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wrtztzsd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nugwgjdu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xrjtcoyf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ltjkzyop.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2lxhsamln.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kaligmci.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cugdusby.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2plsxjpzs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2othxmdyw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zdjbknjx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fjoxcjys.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2mixwzmot.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dkrxgweg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2cyechdfd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lmfyregl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hiollngw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wigakiuf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tjcltmgo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hrvnnteh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bkzyirtg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tjoyhwyk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2egbihdci.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2uzpmbgrh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2plunwvsn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ejhmpvkk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xhzejcsh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2igztjxiv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2grlhazvt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vawrtfgw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wpbdwjrj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rksrhyyy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mckoiqca.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmmemtie.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ohwsvdxg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uxdiajot.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bppmneuy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2iybfryig.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dbghyueg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kwoalwmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tahndjmi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ybzfziwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iubdlinb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jwlnfqqg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ysubklvl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwqnqccu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kagauyne.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqfqwqge.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lqxtcllj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2unfnigoq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zfbzsyxa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xhsfpeti.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gwxajbir.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wtcvbyty.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ahehwjyp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgydpnpc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fqmttcdr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jvhmelco.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2wqlhhjit.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2aslyrwxn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mkylthsm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2skcqtunc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2skxitmgz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhidrubs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sjhyxdwd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfqtgyom.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bjvxozkb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2afzvthnw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2txorgtpo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lwsftszg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2eecuesfu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2biaflgex.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oixvhdfk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ceizmvox.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wzxnlkpr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ulreuxvu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2krvlzsvf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lfargazn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fbpsrjtj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2cesldymo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rkbuwsal.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2waiapxek.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kbmmqgkr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2slruildo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ohyucsty.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dutrbhqk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bsgrqbzj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jhhepnrv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vedvcvhu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kdhuppuy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gvemqbgu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dyknsgkd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ecfqmvrf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2hxeklmbf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qsvrauyn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vywpikxo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nthzxybo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lvmuqxvk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ysiejyzd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fyheleoy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hifimmdl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qvuxhujw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nvrdaeok.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2mecsmqot.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2awqutxef.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2npmxfmoj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vzfdzaqs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xnzonlsv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2othmvhcd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2llbygzwn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hiwmgmue.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2kvwkgmzq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2jmqwmgek.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2njczucgz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zvollozd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hptofwde.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvdcdvq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2krybevql.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dysaxisq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mpbcfdot.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2addwcghb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xtaotyzx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wbtwqvcf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lmyjdjaj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vchkztvv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2veetsqwl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2svjwovws.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kdjshbut.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cgyhsvgc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2auqpmdqz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iustphak.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qpqeteku.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hxjijxrq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2quxugexr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2pjxihrzd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jgskhfij.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xmyodhip.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2zmnnybue.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xsrzeppx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nhdmmssm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ldedrahg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jarmzndh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zspxcsxk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ncefjskd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2tfeloncm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pgnibium.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zfbsutdw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xgnzwjyc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rejtdxul.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jcahdpmq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zgbmkdrf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2vctlcrpi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2uewldbby.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvugfnou.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2igmchabq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2flypunsd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bdrqujdp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2blzreuok.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2opzelmjs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rppkypbn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mdyqafsj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ttcouagm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jwysnute.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zbgaurts.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wzrkwduf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdeugzgt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lvehxiwa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sjlqehzj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pgkfxwos.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2unilmdzy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2itswkdoc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mwwbqqqa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fvrovnix.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjhlmskr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zifhcfdl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2syraijjg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ohyxakna.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mqboscew.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vhtmdkex.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rlhseual.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qbjmdbvf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mtlbnfon.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2atkmgpxl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2cysolopk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2himqhbjf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ffdtowxd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jendovya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szayjomm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ewgohmlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjmmdblq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jurrvnff.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2mcvujgii.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fydybtwq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dfccralr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2jyrxzaoe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nikuuvme.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rrxrsypq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zoedqxta.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2yuymgmdw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2utagfsba.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2kgkfveox.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2osbuwpdy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hvnixbqg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2atcwwocm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2obcucemb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pwfweftq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hnpwzeeg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qucnhtth.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ptfccnwz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yqwxcqwf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fbimfzlh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fzilajfp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2syljscql.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jcngughe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lgcikxfj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tuwhpsnn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ywygcavl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ctqsvlsm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2erlnllcw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dpifgesg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fvhghqga.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cgpfkpza.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jstjbpfl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sayalmgw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2tbwqkavt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2basxooxp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hwkcdpgo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xpcqoaah.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wqvbxsun.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oqejcuop.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gygefegd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2toogaogw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pplwccvi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oxprrsvx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wrjgnmpg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tnuajylb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jywkutdk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2modxvodl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ngkbqbbg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gcrtxaah.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2eehvstnz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edvvrgoy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2duybmira.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zywvdzff.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2aghovkot.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ytmwqsal.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xulbkqrm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wuxkczxy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2golipbww.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mlgyfiui.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zriegdbj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ptmgsbqx.html


<!-- 参考信息 -->