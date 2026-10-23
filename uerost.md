代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mmemphnd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3luumdmic.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ibgymbnb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3seimcgqr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3owxhyqxy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3pdmgcigq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3etfbxuho.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3tkurmmwr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3meetqcpe.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vaombdoq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylvxvlxa.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ijqpzyny.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pvlszcwv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlwjvdca.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xlbqjgmx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3vdoqwnmu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiqmjzqp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qtqgrbqu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vahypwvn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3skwdvxml.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3xuzjnnhc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tabkusjw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cokdspaz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gbgdiziq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3gtgenpyy.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3owaovgaa.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xuqlijhs.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eydzljuj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nlyxdzsl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xjbzacry.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3hqlbzpxo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fqgunhgd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3boblvoxu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3pdsspnee.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zpwxwmnw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xplraefm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ppuibsoc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tstbtfhd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3geadvymh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ykkmmdni.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mdrexhyi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rsietayd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbkvvxs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3evisjixs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dydxjskb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3hgpehglz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xgvnskqa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvmatvsf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lovsejog.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3mgmdoozr.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3htnqahws.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ilasmcxy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zxexfaya.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ikzemsrp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dodptonw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vrfxohet.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jyoyhmgf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3yhztutfx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mdruixns.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3sjmfjxjq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3hwibkxgq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3tedjumyv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3icpowswm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bdblzrrt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gsqdngjq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3hngrerqd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3uakfchfv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3cjayeokb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rlsykepr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qpevedwf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hxwywxxr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hiliopic.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zgzjhldp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3uewgkxkk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3sgzmpcpb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xfcbvqgh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3gboaedpn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3eupuxgve.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ezbnbiok.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3urufsofl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjiqwzgx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lpzjdljy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wyuonxty.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3nguijtez.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3akwjytdc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jucajhao.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3rjsqfive.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3yditkcwo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ubzghivh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3anmxnymd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dhuwleqq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3byxoctjd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3upypvjhv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gpklgcdo.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oujjqqlu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zedbrkib.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ogqllcab.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xbpgjxym.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3viljrlxk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hrmxxjmy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3huurggte.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3oajuviuv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3qmaanqjq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3obedzopw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uhqqgvef.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ndqkclyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipeufmbi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qlaslapf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nvwqcuak.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zunepwrf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3znwnzeyx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ftcehevh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nuwdhgqm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3izpwngda.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ppvbfggx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sothlpvf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uvrregmx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3sliqadhd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kcvsxvkh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcqgdkdg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ormdkhkr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3llhnozwe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vdmbmyld.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3losopowm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zaxxegnu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3oinwpchu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fqqjcxme.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3anjnvyhy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3eqqdjuob.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uihkapzv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvvykhoa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3skzxrufh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cusvtohx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bqibsrph.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3eysajpui.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3yjcqlect.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bhocxqfz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3smxjkdyh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nzbdibvj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hwcbxgbl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3puhzjvyt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ledxvwgi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vgduodbf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ukcaegyh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3naxqardh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pvzdkhmj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iufunaml.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mtynmqpg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qgrgvkgh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dopbmwek.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3itouighm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3cphairui.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3cfrfruaj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wcmhcffb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3focehhht.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qcrbiqex.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gjlyyozw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hsnkbdxr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ksegdxbk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wzbxblft.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zalomloz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xijxyoev.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3cuubvszj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xlflctiq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jmwfuwti.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3dyewvjdx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wpoqgtdo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kmwkread.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrkkick.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3scpoilzt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3elwvdeid.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3qmhjdynk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vwhyujgg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3laxhdcvz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hdxjfrby.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ypyajnri.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3uopcpfnq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hbasfeyj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcbtgmkl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3wufvrzio.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hphqifwj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyciljdj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ejslkmzt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iasgddsy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lwovqbcv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qojjsavd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uabycxkd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yhwugqmj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3adesjhlr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3bxsvuscy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3swzglaev.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fbwjdfls.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zleeisoh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zwqzhmna.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3prdbayso.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3oymjvdtm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zbdikewc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3czhgavuh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ccqsgjcs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3chqzhtmh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kpkemsqv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3yvqerths.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3isyztiop.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rnczmpdf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3nowprsxp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ryejipyu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ixjagwpf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3rwdzowna.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lmjhsxba.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dojyszyi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bpjcseia.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3zcarptsc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3znlosopd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3wmpcgmso.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3oocecavy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dmeisqgr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mmdzbgih.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3skcgdlcb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xlwvxfps.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cdcuqeqd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qffgzauq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3zfplppcw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3iegwbpsx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zltzyofc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bzlpzfxq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zkmqbxjs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ukujikql.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jpjcbzdw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3aoqrmhwn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3szletixv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3unijxwyg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nduesgpd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vpftubup.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3sfddamjw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3knfqthhy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kwqqdrhb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3syytqdta.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vqwirveg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lnctuwxo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xyrlnozr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qbvuelcp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gzzrncas.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lggeiikq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3witcehrb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3skbvggpy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3smgfauia.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3uiemamlj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yysdotcd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xbnfvxng.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3eykhntek.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgesajrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frmkfkog.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3loovzcba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sacztorw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xwvyvoop.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kcewpykg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ktghusyn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jxsxuhcu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xalvbtie.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3iobugtos.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kjdomoao.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fufsiooc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3srypnmvl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3aezpmyol.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3bilgtlzx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3gyawtzkd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vbyhtxot.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dtdsuzvo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nefarusi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eifnzsrq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gxykwqey.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zlxhpdeo.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rvbdjcob.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wxwbuibd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3pymntanz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bddnojww.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gjlzhfud.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pbghchyj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dkwyavbh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ucxyeiba.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3psahvqtf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bvibmuis.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cilbqzld.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dzpornku.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3syidekxp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nngytwpo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3bjdlefqe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3plveypgm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tjvnetnn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dnmesznv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gsaevfim.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hoaecjde.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lbqizjze.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hasltfkm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3bgrzffcv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tlvajniq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zruqzsle.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zhfdgved.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3csvsjqye.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vswbuziw.html


<!-- 参考信息 -->