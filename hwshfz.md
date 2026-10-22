代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrexnovt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ctcovlqu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2veefmysf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rrifvddk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2usaugfip.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2olrrvwwu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdbzrcle.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2axjuekmy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fqurqnke.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2mbbtatbn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2zynteste.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2pdjwtjno.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdfqlnrs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2blewolyx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxwhoppw.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjqzybnb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2kguyexbs.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lkysxdpt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bhjwwtch.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2qyqsjxqk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2xjhzfbrp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ysldperv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xpmgafoh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jrgwgvml.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qhaecmky.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hakafgly.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ofvmckll.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pmtzrrsu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hyzvvtvs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2eyybxehe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmxfydes.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cpybnntf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogstaeol.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzhauaaf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2omkayukh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2eluwiiyh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yizoomtl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yyujtgfv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2xmsooyud.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2afajbdqn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2saqivply.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2iapeeaqd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2muewmhmo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2deojqkvs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2hjmvupqf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgnxrlrs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qtgsaktq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ijeuealy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vsyhmfrp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ifetviip.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tpqzuvrm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mumezsrt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2yaghwlrt.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2aejipxgx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2idwcqttz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2grwoynhb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ulovzyxn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2fnovzmly.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bobehjis.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cuevryov.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qtwczbgr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xrnexshr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uvnsebia.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2othwytgd.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dadezrnx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zkhnuywy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmaypvep.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ytlzoqtz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bayveirv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wzwmhpyo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2uayobpgu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2drzzaudq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rquxmpde.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2coydzpbn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ovhvhfbs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hrxdvcgx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkzasetu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rslamwjd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohisbile.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2arzewegy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ircoemtu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmzevcrr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2sgfrxhxi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2jpamirmo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wykjhvkq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sisstkbp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fqcfgwsj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2emxdvesp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2efmbgqwj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aiqsxjfx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xcogbytj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2zavhlmaz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tlqvolze.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bifsgsst.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kiysgnii.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vgmgaqaw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ueypwock.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2isepwdfp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hglybqpd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kmobbmvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sreunzha.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eepdhlej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trfgktmd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dmqmohlx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ifmvwxgs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfyivngp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fmzpimdx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2plvicwut.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxabbrbe.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hfcaxzmz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vrpjnnje.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2edtkxzvr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vsmxnphc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2segfyljv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxkeecky.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bpqlanvl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2quignhfl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zrvwqcnj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2suzxbsxc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lzektbmu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2nuapmzpi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2bmvfdqik.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vsvbymxs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvwgilkc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rntjfytm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lewvsdyt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yunaguif.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2yanbdrgh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2hcbszfmp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2euwcjlbk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tcnpkffr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bcodsrrl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2uylcmihe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2auqtftai.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2njpbrygv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2cktruyft.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2znzfcuqc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bamhqeog.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcerlsmk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2wuzddgcp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cgcmqyty.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nzepzmnq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jsfhgkbp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uregvint.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ubbbpzdr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xgkqaooa.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iaikmgjm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dxwmivtr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vnupputa.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2eabrlumu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2haffoslk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zaluhelg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cbyfjgmy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gtnzkkqx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vienshog.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hspxvcvi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bmzubpvj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bwunmivs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2bllvaswq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yiimctoz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2iuxweaqo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rpfjyxcw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2oazdfeqn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ybjcalox.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2umdxipqr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qekfrjqa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fznwkdzp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2rularmuu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qdtfcusm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iwkutwfj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hxxukbef.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vakfefvk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pnxqgpps.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2dijzvhgl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gicamluk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2uzivabdv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vwuyregu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbgsvbzp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nnyeneus.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ygbniree.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fqnjnbgq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kblugjon.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rpgsmovo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kehaulzd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wvntnian.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2pljhvhwu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2szlokpze.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pfimfqrs.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bptdtdux.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dmdxozkw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tskjfspy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ekzcrbvk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eilmqhrf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ttdyejxp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fipvjiub.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dfjjyzmu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wlmfbmqy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2imwjizmg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ydbnkxbj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nrfuaxch.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2pzzogqrd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ukcqquud.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2wcgujcuz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ohjsumpw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2hrvbyfvs.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2daegmsob.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2umgmdqbo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2aqkfiyvp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2viwoerfq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2shcjdvrb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ahzttaau.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2apilyebi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hmnhqupq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdeenrtp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2unbnsbzz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2chevairx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfxjcktf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pnhhonqv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2yctvpjuq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2axtexvbj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pzoehsxz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2isgckofp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tpzujqtl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fwstwlks.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekdcfnnd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2yiwtqlno.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2woxtxmpz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lnwbgpht.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jxpyghjp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2iqzdzntb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ykkehbjf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qfhqfsrn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llkckmdx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2befmwwif.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uvxwpovj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jgupemcj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zjuqkbyv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2boypjohe.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bqxbfgxw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ifngeahh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bntpydmk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jnepxaxd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dkfnonqm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ypqolnkd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2znmsvgyh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2awcdkjqq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohjnpnaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srcbfufg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2isvkhzcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybyxvjxu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hnnfgymo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2aczbcdcg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2naqlzmjz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2emnwyznn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2lbpoxmno.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jclchcbh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fahcdowg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ruqzupqo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2sajmalyh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2itzxheof.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ucpwtrpq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2azzogvly.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2edtgrljg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ajekdpng.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2enkxrenv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dembkchh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fevyefvt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jmwecemd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kuxyjbrx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lixdkurj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2fskbyxuj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nowxywbj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mxentbpx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2twqoexsy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qqtomqfo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ymqyxobq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kkzjdmrx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pgggbhfn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rvxxleud.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2btswlhec.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jpbxlpil.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kxbvgudh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tseleexs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yybrohig.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2csxuuknv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wliwbrqo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hzwdjnnj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qhnxzamo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ecevsvrj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yqztufvv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2aitduvzs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hwlsdqqz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2edpqsskw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vmdoyrob.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2korungld.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2attoiofw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2opzdjoac.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bsgvmnnx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tazazbbk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uauuyhnq.html


<!-- 参考信息 -->