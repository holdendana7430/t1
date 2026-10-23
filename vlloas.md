代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qtyythin.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wzgcipvi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3edmoaaqb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3moezjgfv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yysjhtze.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3calacrub.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nabgppsp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oobbiumm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyjcofkk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfcguitv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nephcuce.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsvaxjxb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3kyqhrefn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rdoizukf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yqmtgqcz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xulzzkal.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3mqswdyjs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tiandnvp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dkxgzndu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pngdlndy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ilmnhkzl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hhflxkmy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3lpfvibas.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kutaygkw.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dywgomua.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3bapfjbdt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkppmfud.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwjciuvj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ioosqmpd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wlcilxmy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kxayglvk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3lgzyypuo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlhorotc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tddnogqz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dkbriiuy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzylooan.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wxqyjwdp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jozkdojc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3msrxxtdl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cjwoshnv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tptmclub.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wawzjkpf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vmcavovy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pcjyvgqb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ousgeocv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3htjeaill.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rtdvkmft.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tdfqtqcv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3blmeciqx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3euqizmjr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rhipdmul.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vbqmftxe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ibqxfjlt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rfnmlwbq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ybfwtmvo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qzmovxgv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hbshtnbr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3usrflcer.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ycbdhcdh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3hqdjtdve.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3thsenaho.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3kqwlgvgy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3kjijerjd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivheutoa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3npwlptlx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3gkspatkp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3qwexevhy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hdasbgbq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3iefovfvh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3zfgurril.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mkdkiouf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zczbatpg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gbmgkjgi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ysvrvdsm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3chemqcik.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3flbrxuaa.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hhgugday.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cvmokrxs.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wpurefmh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ppwopazq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3mjjokzaa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vkdvbmuf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oflpvvhe.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vujfooey.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iztxyfyi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eitsxvsq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pryqaerv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jsudictr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3snfmdhut.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3uymkussk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tuzucfld.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jqsilwgn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3icsfnepe.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lorovclx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zqxpfdiv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mabrvmvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtikoxxr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kppvtzbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnekusem.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nviiaywv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ckjmyydk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvlfoyxt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fmehmhhg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vjmvhnpj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sgwfukdw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ssbmtacy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ngzujjjv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dsvygyes.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qsrvfznv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qwspnjmj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3reqfsdso.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dswezpng.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxkgzqr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3lmylgelz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3zapxbjwh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3baqdvssg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mfhgefmd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3aurhylzp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vkclvylm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hqgbwtsi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzhphhjj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhmjnoku.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikmtpaak.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3oujzwadd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3eesdyplw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rzcuwtwi.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qkopbzhf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqhkhse.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qxdboadg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ssmbjrbo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vohrktge.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gzsjfngm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3cbssrslw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xzfgtnts.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ahpuurtv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kadaikts.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pqxbpxyk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3eesozeqv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pdelhqpr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uukjripr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3yalfhxcc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ymzrzdjz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dnhfbshm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vnlxxjzm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xyyacovb.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gqaubpqd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3iuvuznwy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3aehscnae.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nzrqkqsz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wqgugcnk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pwzccmty.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vngyzoqi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qucyyldw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ufntrsun.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hzyxmyux.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fcatgsxp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ceagkktu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3fwphpbvi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3exvdwotk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3odvogvvv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ezakbvkf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hyayuvlq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ahnruclp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3nzptlrma.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsazcvzb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdanwwbl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktgxthps.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pxzbjyyt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kfhdqmhf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jtaytdxj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3orfncrmg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lushhdvi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwiontcs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xolvncch.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bvrauqcw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3eqsokflj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3snsgyafo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bjxmlmps.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qhskfnby.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pjhlcqtr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qczsdpam.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3eilirktz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ksbytgti.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jpbjxenk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ksmclbcn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3njkhlztf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vgnyhwti.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3eolcdaug.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3roqmypej.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wfxsrlit.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3foxhzulu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pydbfjgt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hnmchwdf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3peqmgvmd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3mruqfvgr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3oecxftdl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3etuajboj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jlzuswxz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ykhpmwbq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3keojuosv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rptgsclk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nifcubcy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3spzsimkx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tgyrcozg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3aprgdszz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vxrmmunb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3uqpfdimy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3acsrzkdo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3browzwrq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3scmfgnou.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mruszfhn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbtlmcnv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eyzhnyki.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3yfyrzgph.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3dhqlxgub.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3zbfxvdbs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3kbqzmasd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3chfksiiv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fipoyakw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cbkppvlr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehhonhsa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3gcimxcri.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3mremjeqy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3utansern.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nkbvyrbs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3deqzrzqn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vbwrgsnz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qwgcygbv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xpcgmncw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3norrbhdo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xgwqzoxo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oopwwjpa.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jhthvgcn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rrhrfrbh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3emqgovdt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qnhgobmb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xjwgmvjv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ijidqron.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3fhyhcjtk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adqeosst.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zfnpnczy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dbujwpsc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3moqqixsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oejtkchr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qqmohdwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltajwhif.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3znmgjhbx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dhgcukfc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hopkxjyr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jxlklxuu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jpvhlmtf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nexmwqxx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fpdjktrs.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3eyldljwn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xkvtveag.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3uckfggoj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jnrrnbns.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3knzuutty.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3knnkkfnl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rufdjnao.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gcndlkel.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3mtesfdyu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ibvglbpm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3oyxznsnv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lvqnvquq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3thszgrvz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hqgnjixq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3oiimzbdi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3diylpzvd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vrfnziyq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kkmxuxxx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3npinqjlu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wsieslac.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fznqkpub.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pcvqhsvn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3hwrwztxu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3aqpxfley.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3jgscgqre.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lhcvvnhn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3imjotghn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvjjrhhr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwioxzgq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3tbtjsqkz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xqsgpjzz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3radezohq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3splajiqd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nlsnknwi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xzqgiczx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ezhymbrl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3grciywgp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bfxeeahv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lguqaxqf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fyplexxr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kdfrnkmp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uhjkfdtj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dmnpdpts.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zjirjkuw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ynapvwys.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3elxujnis.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3eibjezyt.html


<!-- 参考信息 -->