代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ylhtbfbs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ehyxooac.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubbmizlf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fbjpxelq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zcmwmvmn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnckflay.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ehcbgyir.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2unuvtgul.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ddxhpnyt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eosbduki.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpdpmjdl.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gwdfgibn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kfmidqpt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ubzeccio.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gffqwxrc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hrknqiwt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vujfuuik.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xtlhbhey.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uizuwosc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oqixqrpq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lsdhoqmh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jgckqwsz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hahunwwy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pfwqelew.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2lzlmptpg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2tbdxnzzv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mqbinpov.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xwgywodu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vqhfmhki.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zsgrigle.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pzjfworx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nyrrfmyk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eufaihaz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2fjrvkcdb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2udxwnqch.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2epfixztp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ylekvnaa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rqfthpls.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2epyqtqla.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2aepjxcmk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2txyydaff.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2azumwfhz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2kvdhortr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2wrzpkglr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qmthqtvs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2efllowyx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rtmzrqxr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fprytpot.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wskifvte.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ymygmduo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tmjxncxg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xzggnuga.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nfkmkqxr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tkbsigcd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fcemdwnt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mwmtqven.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2apuuovgq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gaaicwjk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ypgundud.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dgrpjjrs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2voiosjce.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2nknzmlzf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zpjikyjs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ebizcpwc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qliousnj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ynixrhce.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xhbewsel.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2xvstnwla.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hmritbie.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2eokrjdsp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ijqigxen.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2gxzqvytd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysevbyhj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wbftlocx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpnhqkgb.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yqdhifkp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2pnljlwlf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oeshwoyv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rzbiiufw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2dintddjn.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2cmkrazwo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jntdlpnh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mfuhjpax.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kwpadxgs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gdqefkjo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ovikdosc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zdqrnvni.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nkevmkfw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lqcrowro.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2nvxxojdk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mzdcsvzn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qpoyucqj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rwmyytbg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zcejpxty.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bbhauemn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vbdenofa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgyhthza.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2bazvvbdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqvcswvn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2surgfsiu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2faapmvif.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xvkshbxl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rtgotyme.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmjjlkze.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hhzicvrr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rtinkuac.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2crpmlmlv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjsdwxqr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vvhfnmjt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qmamzliu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cezxwzog.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drxhdzih.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obyzwrnj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2svriprnb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2icdagjtt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zbbbhqfg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uvqpvzri.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jeesiaov.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2feldjdgx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vvodwvxj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnopxmxp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzlimpe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2hkaygtwr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rxtkqwnp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2byucsyrr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2vkcesznf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2atnqhzlb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2fuugxwvi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2alstlqak.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twyujqmp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wffcefrp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cqzuucof.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2zaekqtpt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2txngzses.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wvidbjpr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cdnmmjnj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2oxgvwafw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2acnepmav.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ovqlxaji.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gdvfuruc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wxqqdcvl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tjfkijke.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xlrbtior.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ylnwvgei.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cltqgfgu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qqipywrz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xlztbqko.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dlbvuqyo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2khjpazpu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2snbdfifn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bausohxp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pcxacijd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2aywywvqh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fwqtusat.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2deevqvay.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2optfnoqo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nidckhlj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2evblexma.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2vidcdykl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ssfnryrb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2qnpsktob.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2swzelazl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vhxambhh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xatavmzr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsakvvts.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfftidbk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiwfifzm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2tiyjinff.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tluaqpyy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sgzftjnd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmdcmlcj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2icrgyjky.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2talejhnf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxdrasah.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pypsmhfy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xviokkxx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2odkpmysw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2sztwhbym.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ahjpkfyq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2iajbvucp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2wvvizgdm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2twnzrjoe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ktoezhxm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zzdauxaw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2obyrxnqe.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2swzhtdby.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2amzrhwzw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pzityqxw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ptnplbtp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nrzmyqer.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2tsmzujfh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nrzrnlzr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dgjribzj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nqtrkapa.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2dfyyrijl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2bnjhxbzf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2pjhlgfwg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jxskywdq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vtizxodc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ykrzlcse.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dlxeermw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lbtlaplq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mjywynhw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gzmeduol.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ehgtmjxj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dtmicnlq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2pjhkgock.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nytwlbxs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yatexhoa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtczjvzx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2itrjvcxh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2igmvlbkq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2faixetxl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2itcopgme.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fhfqixyf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ozfscjfz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2glhofluk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ncqehowi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2btafljtj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xxwukrwg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gchnbtdf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2drpprkfb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2knqamluy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vhmooush.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tpkbtfdn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ngjxxatc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hnfmvwuq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gwcdxlyy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycxzxavm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsdczbux.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bgrixgxd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rofotlbk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zbceitvc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ljfzbkhg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lxnicyuv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2lwoxhekt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2espbwmye.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fzakhops.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kthxvcma.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkzcyibs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2lkozqxtx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2phchrnsz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbbevnyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djpwbues.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ufslgolq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghuwqpth.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gukeuoau.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jopovfqn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2krierusb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cuszmbbk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ooijgifr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gxyuxwkn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2brkbwirx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2anasuhgf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zqkvogie.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2csnjniyk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dixqwrrx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yvfotbgs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmfpudzm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gdxiaprq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2uqmkquxz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hmczqltq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mhbuporz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hyvzafkl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ksfdqhsq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mtrnrpaw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cuoerqpg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ctcarwei.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kqhvmiee.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2secriefo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xwpsqqap.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2asqhcdrn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xemaelkv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vqoedwgm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2icxqfjoh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2yskoahkt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pufwaipg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xxdqzril.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cqfthpzh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lpdpjtwx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iugbttrq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qyjxcwel.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2twutmaay.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zciktjhi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tfijbqvu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2klfnyfoa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hmxsrhup.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2fqbrrqdg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dndcorlw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mfmgncff.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ddwxvkal.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mzzmpipf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eebvazra.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lbdtxdyi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mxahiekd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tllimtqv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wkjvecqb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gfrnkffd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pcyezrok.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2snigbjwv.html


<!-- 参考信息 -->