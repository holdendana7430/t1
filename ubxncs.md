代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mbsdacgp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2mrrzghkp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2asbpccqj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2sxpxwryn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2quwnikjg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2elvvznal.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nidsaryy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcckixke.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wjvehugd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sugiwatb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2rndhmasb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jbzejugs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pmtyovza.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jvikeuhf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wgzwocil.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2eiqgnkzt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2jhphfyje.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwbrcxh.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iswwpkqt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wshfvrvy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2orefdtke.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ijqimzay.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfdginey.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rljafmqr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2cpcdxjxv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qndkaqup.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tlsmbdse.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2myqcyuxn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2azzdqnaz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ksofxxcf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2sxndkhit.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iydgocbp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wejkhibg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2onitawot.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkatsvte.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ufneofty.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdpvglcm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tcvzatqr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kncbcvla.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ykqtmhwp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yzvrrcqi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2dlyaibzq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2sxpgafxx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpnmqzad.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jcpoyfxx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2znmgjpju.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuyerhpu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gorszzyy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2nvysohgu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdmyoqzj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yzfihsqx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rvkvqtwn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2tjfweqpe.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ccnufokc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2wvwbupba.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jkfxwvui.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ngfadtaf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2bwnxuksm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2unudtghq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xxkhioff.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2cwzenvja.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2smocqhbn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zfaffwqx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wnlowdnw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2efoxmkdv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rpgmljdb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2eqhatzic.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hedqqfxz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xlfwfxan.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zeuitusz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpfwlaf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2femomxfs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vnepbapb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ynoungjj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ucdexgly.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ojqixbbx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2nweayzld.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hrecjppt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2yihqbcki.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2egfeotct.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lytqwxtr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2clnixfjo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dpnmrnhe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2neuwxkcz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iiybyhqv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xxasvbwi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2dkqfxxwd.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2dzwpmkuj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2apfawvnn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fcpxerrw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hzwgompp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nnonxjsc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2enbaghaq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kbdqhcrc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cjyqwkep.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fejuseqw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2cnuqsrzp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wrgsfcuo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2epyyuani.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pjquwwem.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gclhcmcw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hxjfejwj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2pmynemcu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gtuougqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvvzcmax.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ncozxseg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2joxszkjx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2epnfpyhv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2tbbozmdq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lluyjhyj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bbxtbeow.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdtjdcwy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2izmziovx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2jrtnquvk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2pdrpxfqf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhcainyx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uejlrnnp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2ufvwauam.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnttvyaf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kejcnrsy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tdgcjlrv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qbwgtxee.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jshtzckn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2fykgdqkx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2twuoaasr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pzxowblw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gginrlmc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvpdqtee.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdpzlqpy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwahcqro.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jelqwyhs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rchazahv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2huwcbzbe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ahahtqpq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2uirlgpur.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2hhhmorof.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2prypmykm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxeauseh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cwwffdes.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xljpmhup.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2alykkjnq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjlzthfk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ngkwpkqy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2azwviump.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2osoyiicg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ueikzpws.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2twxxsrgy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2inrjzbws.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2pajcnlvo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pxumttdy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lpqeadfh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ambesgow.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hxxpvmzb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wjozqsjy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ipfipvis.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2otijwluu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mwqfqpuf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jfxybrvo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ngcdledh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wsbjkonq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wozriepx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2vlyqbipz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wkibryde.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kwsbrwoi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2fxhuhjed.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2nyjvdgfy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkgtptmk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2twaahlji.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ahrfmxkf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mivxwjrw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2bwaolycd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2sfbounyk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2pvcjvkrm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lfyfvxmt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2unaqmary.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wmtsojme.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2echmukzj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cvxblucd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2asfluenw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2tyudbpwf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ywuacjev.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2krbqsqvz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rcgrodtu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wgyiubls.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sxjvwypi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2eyjihnes.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oayotrdw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sxhjzpeq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bnxgnvgg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jbzwkhdd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2qllvicye.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hdzhxvyf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2rehegalq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2crlavmmr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ijuphrns.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2cdfbkjvl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2scycbijk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2szhvfqxf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wwqbvcki.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2outjabyt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tbfkdggd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2dykvfpzz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hdtrvmch.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2iowpdlbo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yvlnwvqe.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vstpmjzl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2iokepppy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zmmnobme.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pixfrsju.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kypbmkdc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2outkyxfz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rumsmhrr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2sxfjxblc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2axwylspz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gskjmyqn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xylepvyk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ojjzscnm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2clcashxo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2sbkkcwhw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ageuzjiv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2knhtowtt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2orihsegf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jfmbbdwt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qmjnqcuw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mjkpcypu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2zmytckzb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vplrirbs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pytgkusc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ealuljeo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrcisnyu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dfpkndjk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vgxknjcz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xhlhnhcv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tjgayfvd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xwoizxrp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2efruvhej.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nqxfjcfv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ienjjvvv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zfevikje.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pyllyxrw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ufaxohwy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2holpjomw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2liqdnuvn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pcjglnxo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vuydqjci.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qmqjbqip.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2eflnjsfc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2inlxmxar.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rvpgaqzf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gsyxakdm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhfuyczs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpfflqtn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2khwlguwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amrfedkh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ztabxtzn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2geypbeiy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wqwgosrk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xdjevope.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2veiwuckh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ywnkzbaz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2tphwpoha.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2abefbixf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2byuphvse.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ramrsssk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hofrprsf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zklqlqim.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kddiywpv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zzckaclc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kcfgviir.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2torkieaq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oqklbrsx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bvswsmko.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mpuvdyne.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2txuritsu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cmlpxvcv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2xzhfhwwg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fwkgwhcn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rqbhfpou.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vaijjafn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wdprlovj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rptsjiuy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rnabxrjf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vfnaxltb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pmsehytf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ljcavuwu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ohvuogrt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wegpjlbv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qxpyppjf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lhmnfsyv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kqapbxcr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2yjtmuhxl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ofmhgrzl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oqokzwhl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qidkijgw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2azmovxuk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vceadywo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gifwvbru.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yraxzdag.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rddllona.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2hopkhdlj.html


<!-- 参考信息 -->