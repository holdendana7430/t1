代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nulfolem.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2dyeuzshx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2djbktuop.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2cdzzdzlh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttfkpzkw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2encsvfpf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wxaimqpf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2bhtlpzzm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbtevcoj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfuqcffg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxshtmdv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2pljkydxj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2esziludj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2obfubnxz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nchfwmva.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2osadxxit.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qxzkaknr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvdtnudy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uihmjztm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pqoayoja.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2nftkgrua.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2liplwptl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ascgllhf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2cdoslcia.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vmdyuuyp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lcxskjjh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hplxkniz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iundcjmf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ahmukimw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nzoslers.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qcgivbeg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wxnqgbpv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2yzzivkno.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xxkihhaf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmttguqi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bshuanvz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzpigcdf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xkufyumk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ifcjtfzz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2dbbhimjk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2gryzndqe.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2snnfswui.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2smppomzb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwsfwywn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rgcopfdp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2anlhgkwx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cudicusx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mvywdjlg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sodchdsy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yktosbry.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2igytxwxu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2pbgujjlb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wujwgtgd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wlrldizb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hxkftqcg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2wxdxtjps.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xsdvsktq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uolgsjre.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jtaxlvah.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jhrzwwrh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ewyzjqnm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ovleivhq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tbtiiwto.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2akrisgwk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jvzlnxon.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2tokddywl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bikfnqkj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2uezxahob.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gdokddmv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2madmtlwc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2iyuuenzq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpcigmu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knbwfwgw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ayioeyvf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fawjvcnk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2qmicphip.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ydgqcrke.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yfjvxrqn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ltpksafh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2heejuncr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2seukrkkd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vthqeueb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tykcdmxl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2qldebnok.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rayfxiqu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edqjvsla.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2aowmfvar.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mmnxatzi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2raeyvtpq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2okthqbyv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dytvsjmp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ulsdpkls.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pxjqqqfc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zvmescqo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zdrtzieh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dmtuquvd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2assizaxr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rytaxdci.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2yjimjdsn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fdhssuay.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2elokeetc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2nlzgegpl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xalfgdbj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2agellevr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smwfcevq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bjjyaoeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdxdhgwq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qiywdzdn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2sqjtvlvs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vovojeir.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmzwaheq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mppaivpg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2diljkoqa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rgzkocqh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pxftxygc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ltknknio.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fvxjkqmw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pbqysrdh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxscwbmq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqbjmiwh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlgzmydh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2bhglbwzi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2lnrauhsb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2dugtqqsd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mqplizyr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2sqssvdte.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2zbweuqhw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2munxjoaz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhwbwapw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uxpfzssx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkagivqv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2hataonrx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zsfaprxf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hsmowaww.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2soojnwdk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2bhbjmbbz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nlkupjfh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vrwmykwz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pasiglxx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ookedzzr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2pgnlmclp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gzokrchq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yqewewrz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mzxjsscu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2noyvndlm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2inuhlvgx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dgnpgtuk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2twuiywef.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ggmkeqrs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yunjuffx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2azhsldue.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dxeetxkv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kfxjhyrs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xhfbhzhj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xbyjnhxo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bxyjtgnm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2owzdcvzh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qvymrodl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ideyoskd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2rakxytdk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vaikgvjh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dclwssdr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vhwmdsbk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bukgsxgj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vsvfbwtr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ykuiowax.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2frwklwlj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2hrvdlvlv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2pihlkodr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2iwtiqaxo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kfhmnfjx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qbjcbmmn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwjhynvz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoftibet.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbwdgpmo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2bfdownyo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2uxikwzwl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwbrdpwa.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jxfsztlc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2csdywqhf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2terctnqg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ynuroeoj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zbtsofbh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xcwyuilw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vimboqyd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2chwugpzj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2piihwljw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fdhilkik.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qsbyyuiu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wmrrjauq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2sbswnfiq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wnaklivk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qjozqjgi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zutzpoep.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2grqfmxug.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2noilbarc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ddbpzuoe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ztwavppo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ggtncqvj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pbutwhbz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uozbtivf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2skhoitwc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jpkbetkt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2sqifhmob.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2winldavr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fsmabggs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zumrrvek.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vcqaohhk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2uvyyfytg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2adbdirbg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2uzmdoivx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vdjsgmor.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vpebyofk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2soiwjmyy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2sscgbzlo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jvvxbytg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hyprnonv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxpmyndr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2xcufeafs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uzotuauj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rgscpory.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hmyfnpmw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gsdwgcoy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2thcikdmp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rlidhzky.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xklbkxul.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nfslppkx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uuconeue.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntzdzldp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ppvqehlb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2iabevdek.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fmgpufkm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2pyrqciut.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2otzozxdo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xqmpqpgt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bajchypr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iexkhvdo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znmokoas.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ruarckmi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cusuiohz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2yxdjdjvf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2aafiajjr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2erfoqflm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mbxcwvqd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2clccvskk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ziqphsop.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2btuzaheo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmenvulf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2yfmdvjhk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xqtyfjuw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2tymkumpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mazsliel.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bnmaswgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpgwovef.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2herptpud.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2yzflmdvk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rvbhrxbh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lesijwaz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2frkluatz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fneubqzb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2pmblcswf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hzmswbrj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ogycyofq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dzvghhea.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ulzdebbn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2aeungtbs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ukvbqucp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gfnzdhhl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2efiolqal.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zdxjvvdr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rtftegll.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gewzmvoj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2iocboofm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgglyum.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ngasxwoo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2xsieoweu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rcpeassu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oetnuket.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2cqsrehzb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zojfgxja.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ofxpukax.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gpuxbvln.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fkxadkas.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2owtfmqbw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hfwtcfee.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cvgpzfmy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nxrgrlqz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2goinicra.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xdfmcwhe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2okjzesyx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lhkmggws.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wmpqadcv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2poqtojya.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2arihyczo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vkvaklns.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rnlxwzxq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uiqbihis.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2epemkhqq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hrxakjyj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xthwuaoh.html


<!-- 参考信息 -->