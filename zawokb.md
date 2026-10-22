代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2smcccocg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkuyrdxh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xwesqtqw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yobxndjd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ibcekepa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2szvrzszb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xzdmatae.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gpuunxbi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2nouxtcsj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2djtleopq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2egyunqlw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpgdnsdf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2lqsqmhfi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvogaxel.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ynpdrmfu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2tadvflbq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wttmszvc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cnomqgfk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ntxpmvlb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zxicqluk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lzyocggt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2upcagcmb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cpxcgsuw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mhjtiqgw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2emkzialw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2armgebgj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nygasydc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2culriprm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gvijqkcw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zpcpanub.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kqmwfaqe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2cslgifnq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ejurzvyw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cfswrdru.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2saihkcez.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fcsyizxm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2swafjeah.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ygytmsdg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohmvczir.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rzrxmdiy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2wybvqfzu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvewvqhz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2cgplilqp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jzbiajwn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2egpqivjh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fmpmmxmd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xhfoedyg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2aepsokiw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2chaeffbv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nunisvaf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2atjmxfcz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2hqbiarhk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ngheoixf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2txaeltif.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zsarygkc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2geyjvvqb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hngyjdxe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zsigffre.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dihligze.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2aczxrnrn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2gbhibton.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2cmkpukfe.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kcxysrys.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zbwnmcxz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2fytjwnkw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2fepihoqr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2akhdqzjg.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vkiockxf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ykjtpmes.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hjtlpprp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2qrnqfted.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2clxfqmtm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zzxhmtzp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmswvugy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2keqmldxw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxnhpqxv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmdcqkdd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jnsdpjil.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2oeoyvxwu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2fbepkqfx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2meikihxo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xphlwvsk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2csyhbsfc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zzbqbwjq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2crukonwu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vpewbmyr.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gfbdvptq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oxvlgxct.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ntdaxsom.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2koonfofi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zehaqznw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2guthhuhd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uhgpihcf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2niopfvkp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ccenqdbv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jcizoocv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkubhffp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yvsfdywt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvbjmrqk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cakiyyra.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2bryqfgcp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vqqagjyu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrhmukin.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ceqdusdy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qlrgzmwm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jassobiv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2amvqdedd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lehuzxbb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vkghtcnk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ywymzdji.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2bafsxwhn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xhcerdmz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kslhqzbf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mjbdjgta.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2szygvale.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2inugwnig.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lhlnbfix.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxccdcim.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cftjbfri.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zrtpvbwp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2udusspcx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ieckdyrk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayywcrjs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qbwjryid.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2mekmhvua.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2fkknrqkx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wnfrdljo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nvogyrpi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pbqppsms.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kpjbobim.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hphrwayk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2jcvdhnnp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kjczqmqf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tlvlrrvb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2trjepwge.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2tzwcqyvq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fgloytzm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dfucpqwb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lnsuisew.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2eycmvqyc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2qxgyewyb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cejuwprv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2plrpxczq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qrraxlan.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2twtlsiwg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xemtacya.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zgwqlvvo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rwywiuke.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vujpkehq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vcijniep.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ygvmcdju.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jlcljrat.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2raolmmvc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fvhpxqlg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dsyisioe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aliwnfwe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2zzblqwde.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2pkqwukwf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2gbagrxkj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2atzmatmz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wimpymox.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wqsqixze.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wtqbziuj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lnxprsxw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqitdkly.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2exnmtyzd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ervqcvqd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2giduidxx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2krdvdoph.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufhbzada.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pmbssjmo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wgukscqv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqtxdnvd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvpwsqem.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dioyhulm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bqrbzyzq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2snilkmxd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cnmdpmhx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjeqqjnz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nmrsmfrv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lmtbspra.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ltoujckh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ijyzcwvg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qspzkmko.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vpgmodbx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wqbmonur.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vyqajkrt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zkdbknvf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pemmnepn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xzczxkoa.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2oomxhyca.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ikmpzskr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sjshwvlt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ryaqsvnc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2nwwwuxni.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wsgyfsrf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rsqngice.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jnqygghf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bnichdep.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2uhlkqtbn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2hgroitbr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2spkgincf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ivyuafql.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fwiphmkp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kyciclqk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qjetyhvb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2boxkvlky.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ysqxzfkp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dcwquzft.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxomsxvn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pvvtzudk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yokidyvr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2neqwechw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2iagmztjj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lqzbklvz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xennkqmh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2subfvzuk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2bflutfkt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fdlnilxk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vvicfbxn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaimklwt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekmwqbiu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2uaymtzon.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dxvhpjmf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fpmewjkj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ocgvhagz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mqooghcq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2dzgacpmu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kqgsyrvy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxxchynj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2woyaprmp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lwwqisxo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hseihnil.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2maahpsvv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uddpdktr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2dxnlnfec.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2iercllzp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zgiddwjv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xmzntewz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tzjsvfpe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dcppwmxp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wovnwypu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nnccubtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oictiuga.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ozwnkhts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvtlzomt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ctdjtctw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zrzdpyrv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2juzmjylm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tbgekcwh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vxfacplx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ttarzlnu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2aawxmnbx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2carwjhqi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2kllwbnwt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2pijxznep.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ppkbfhoh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vzgrsoys.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xmeavmrs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mimlnzie.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ystckjpl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dpqgyusd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mkidmpij.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2khefsvle.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wznjaksm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jooblfzs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2sppzkpit.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hibztfbz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2roxmnnwl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gwvkajvg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mcvcqhwy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ootyejih.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kzpfevwt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jwbyhwpl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kntojbkg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ylotbftt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2abrvhaoh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2drjxxhjn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fceijdqe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2uxdxaram.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zlyuuwzc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ikgyonpp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2grduhecv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mxoqhowm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tvtzefgg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fzsbpzmq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ofuauinq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qbrdnzju.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xmczezhi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rwyolggj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2adrytlws.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2spggajpg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2azorupae.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lncltmch.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2oxukwbdp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mflgkxnx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2rickdemp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vnerlvpz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hgeefjjd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2trsyvzin.html


<!-- 参考信息 -->