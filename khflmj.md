代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3edhhttck.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fqfqskxj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3beuhknqh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3psxsvlgu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyiubncv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kkfrpcnj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aalzwtcu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfyfscfa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3vgkwnlsc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3orkyovut.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgqavuun.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dndotmcb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xbkueiyi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3istqxrhv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xodroixa.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jdjghhpn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zchtshnu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jchjcsrm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3bpbdapyx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oayiufob.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3cnyobzkn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3wyunyasm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ictpnwjq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wecgiggu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlyajhog.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hyazigew.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wfkqzgcm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lxlqcqbg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsbxrvjl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ywngfzcq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3wqziyppu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3yxpyjstg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ulusqqph.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bzfmmqpe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmonahbk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3iudqkpse.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bnarmwbd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlamylhm.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ifpdciim.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ppdaccuw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3szccyzei.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qwnnbbga.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mdquempq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hrtbfcma.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ftgpcnst.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ubhyzumg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3worigvid.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uxyhibts.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nagdapit.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3kyxfqoil.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bihwozce.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zdxkqqjm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wdbivzmb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3owotdagv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ylybidxd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3mkulkvvw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jkgaqxeh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jxvwczrv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkxgoxra.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vqvnwdgx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3reboxiiz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3sfixsyfa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3davizkbc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3kthyhbxa.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lhmdpkac.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3hflznrpn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ytpdthgi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dyvvgamv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjfrwbxk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sivzxtzb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3crpkqjzh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzmfdcdi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfbxgmmg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mujiujsp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rixcgdbw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3qphdmawk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3itqktuyj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ahwoujmz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gaclemsm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ruxfhlbb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uxfhiqfh.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eguffcbq.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cicqaeiq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3goxsqlgg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ulvzhkmw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbhvegoq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tefvsara.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3phfwftbp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tsmsobnj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3pvynmqwl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3bjvupxgh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vunrluqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjzovqmo.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3msqreyli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qacckjsp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zxwpfnho.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qioqwxrx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sjezhwol.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3avzwjpya.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3evsqwznu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ncrihpmn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mhpnqrzc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lyfpulzz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgfczllk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3faxmyjpu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3rcxcohtg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fivdnjrk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3giczbqui.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3enyaeyvb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3bokjxzxp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgmfckvq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dnyhgont.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3fvdxwtod.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3iwynrskt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bgvwvtnd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdygkfjr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sccsykup.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvqkotum.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3zegkxrtl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mfscjfyj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gkhjwefp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ugckdtpb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ctgwdadg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3bbdrkkyr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mwuinrxm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jhplcjfa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wbmwryrj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fybaqudh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mlbqqrqb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3utkyjhtd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lmjpjcek.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3hjnlchcn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zkjnevuu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3thztahvc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nhljkvsc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3boxbyeqt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vlbzrsht.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xfyglmed.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ofuiqslf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3kjjjlfwq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3enseghdf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ebikzawq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nqqboxxg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eqjafzvo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rjwmeufk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yrnovilt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mrmpcmhh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3igssonze.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xkfysurw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jacgsokg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hysdlzgv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jypkamso.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ldvdswtn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ejgafbau.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qbkfsdyu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fgwdrtjq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ngidkrvr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jlvquzlh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pbfqcksb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3biedqxqq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cnstvisn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3grwrakgb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvgtshjq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fklkwyxt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vlpewygh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3aubxeolf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpbuojpc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3eawwzogl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3osemidqk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctnnnipm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zscjwgyf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mnezrrld.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbyesgnv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qdejjtqy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iepdrlqz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3scnxksfu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fevftmuq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xtsooemb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3efsjtpzg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3synxpxjc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jiaylikw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kdqlynnl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kewvbcjn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3fxyfnpag.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jiaprlhm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jisdzzla.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tedkktpr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nfbuqiph.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qldxufda.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3mleizvea.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3psscfkap.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3bbczxcav.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3sdhvrshw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3kqkdszfk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3okwgthhw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bwkpvfef.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3hkztdbph.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cfhivohi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ifksxcpt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3yromhqmk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gbsxcofg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gbxtrrxx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3swdnkbkh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3paptifez.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qksnujva.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qsezcsbm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3manljrdk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uohvcnqs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykiynrkb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3qdebrkzi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rvrkmjyb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3abpbcsmm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lonhjsgu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wouwyqoj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lveerikp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3psldszng.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3axqamnbr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylmjytok.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3eidymomf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uhlsvzbd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3osbysliw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3uojwnkqy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3tjfxzevk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3azejojtj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtbshkty.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shuezhah.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gisozxlr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3eyrkjzhh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ywfodusn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ttlbrfju.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3oyerutcy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ykduvehq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wfgjxgcq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pwcdtwmz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3byoliacw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjbbfjlq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hpnurcan.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3awcbxvxn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fcdnmvbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nelrbiue.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zxbzxbpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmrxobwr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uaowvkau.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vefhpsph.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ypwqwrkg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fdkoxnzh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qqyoixrz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3oftmnpbv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3gqcddoxw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zcjwgkhj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3inhogjwm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ifmpksaq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kvxwqmox.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ojgevgby.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jfotzgfp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nbaobzlk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hkaaaqlr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ywacwgec.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3whlfmzzb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3emuqktqa.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ykrwehhg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wtpbdpgc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3aftqyulr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qogxtzif.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lmtaphcp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xhypvvhi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nhhbimsv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xyirxjpi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iuhtipbo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jcrpmxbg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jfmanzsh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ordlxvjn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3cyqnkkby.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xefxlmoa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3plzbsxxr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gkreknfa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gnqhiznt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jvzstzqy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bjxquzjj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gtznmmga.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yabgztfd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rosgnolu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ghftzywh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3aqrultjj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fybpaytf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cjohdaqe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rgqbddnn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ibmportm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fsbomara.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3glokfequ.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3okazkaws.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tlqyhhxu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3rnkomqtu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3askrvrcs.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nzwjxzgq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jehwrggv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dynbhgje.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fxocvmwt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3okhjgacr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wasvhpai.html


<!-- 参考信息 -->