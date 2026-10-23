代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3grrwcskt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bifyztvy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fdngpuam.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3icrbsozz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wovpihqp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3rprdamjm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yoewmdoq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3uzkufxcc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3klklsdvy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmpjmmto.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ofirznxx.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3emlltbim.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ausftfhm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpgnblow.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3elnjnknp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukagqqok.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wehixghw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3baqgfppm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcrnmqeh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mordscwp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3gidxwqbs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yxnlqrmy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nmkvfkqg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rsyydple.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wcvptrmx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ezjjpfjz.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qcmsanxv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mdfacyhg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3cqqahilm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jcijxqiy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oetwlzda.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3elgvjfgy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zivbjqve.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bedciiwk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3fagakukv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3htuhlhlw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mkdiijto.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3dincvvdg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3iunqchgn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmaiopql.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3icsloeyt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ykwdoamh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3essgnpog.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mohuhetg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3kfupnnrq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpcuixju.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hkqbdmvy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3uoetnnim.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dvbzbjjo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bdffjygz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hxwupeiy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3obcljsdw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3rtjqdqyn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jppsjefc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ixzvtnhd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tpnyhfco.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wowocosv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vblynrgn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uuumfvcd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hvpasgwy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iqavnbyf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dfvujung.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zkauvjbk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3lyqiptln.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yemgnbvu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3vnivqeri.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bvtrmegf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aapcgyuw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kvetqobw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3neqshxhi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3oqgjfjcm.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wucxyruh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3iqielwsx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3aulrxupw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3axgatwwl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ehtlgbio.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nflzuyfo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ktfmikkm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jmvxqaei.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pxpmwism.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xikhlfix.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzmsjtpa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3oqxqsozj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3poidhdfl.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uwczcsxn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jthevrwz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pratrmxa.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3abdbpkxg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3umqmlkou.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lcaeuiuw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zzbnsnoi.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ktrgxdlu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rmudtrbp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jpmejscs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3okczymab.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nddyflzz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mvucarar.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ztflnvmj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3mdvdqgxr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tjqrwfhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqrwrrge.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pgagaoat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vineogrw.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3arhvgoyy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3omjmhpdm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvlpfqrn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoknsmys.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3afnfybji.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieabmqje.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mlvuqbph.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3bwoyqmjl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyerlacf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ygdyiugz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3vyuagpfw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nfywwedr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkdvcpwk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qlzacfma.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dhjxjccp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3relynqks.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3jjheicqk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kuahyofn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3bwzkdsma.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rewmjnob.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3biqhjtkd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3dbtftyhr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjzsboda.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwngsifd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mwqwoffx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3onwrqozl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3mxmdedyc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tsjjmzdp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3huqhfdbi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3sxkplakk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3etvddccf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3eshlzmec.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wuabyjle.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jfuqmkyc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mpavoiat.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qdiitzvu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3udwxiohi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3godxvfor.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3tsqdxijv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3azdnevqo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pgirynir.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tqftwlwd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3thbvaofw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bzmhhykm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zaipbivr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kpblddsf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ivbxpzfo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3wqczvoit.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3niegubop.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nxkxnuxi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fzlwzjzv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cotknufz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xhoocpow.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yjrpldbu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3seoahbwx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ufkctdgf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3opqkmtcx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lzgtglmu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wigyufzr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jfggdptl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3hzdbpguv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xfbygzbx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ohrvozkm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3appsogtn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3fhwcdwkf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvhcwjyc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxgtnelc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3npkntfms.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fzwzljul.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hgopiutz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwvxonms.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zybsvdwt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3wzucmdwh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3izocegle.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yeeyypvh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cxdqosmg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tinoamix.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejmtfpta.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3rbujvadc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gkumvllw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qhpnsleq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3phgxhoha.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3uxwenznm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3euudobel.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kpttcwhv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3navkuycl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3knwcrdhq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gxhsrhlp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3azakmmtb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3thyxgmrj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ucrutluc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jasgbove.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zlqgalsp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rjljbeqz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lstivoon.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3seyjhhgm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dyajdkut.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3sasyajrb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xcuytljc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3cnqwzboz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lgxrvpzv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3telwsrbk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lxxdbtbd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qhbxtmcq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tjjjwniy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3tzqksydt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3bzqgrhar.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3onkyerwx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jcmarrah.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3fylpcyxy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ibmydzkw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hkmuwqhb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzyfizji.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zpbhjgjp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bemezauo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3tlyfdpfg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ymdyaubo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zdachahi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ubvbjedq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ydwgrsem.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sqcsttql.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wdgkuxkw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3onnhuipo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3yqcirzjy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xgpprxbt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pajhguzg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixjytxcp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3yqnhcplj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lthgffit.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rzifpaem.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrkrjzcb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nibonxoa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rjfqbbfc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tgayumuy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3efzrwwqu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ootlwlob.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3pqpwzczh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ohpjjmfl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ydiekhap.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3oozsxwbk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3iajwkexm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fqdyzejf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3izwghoma.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3difumszh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hsppcgxi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3wthhhawk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlmaphcr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qfkdocts.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3tysvzati.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ddkjrvlj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jhleeuim.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dndrvgql.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3orxicelg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ggvuvxim.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iulkmmdb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mowpciyv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ylhwpusg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jgtbblvf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uclrguxs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pqezzvnu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rqzwsjlv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3guqwnssj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3czcenhnr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nxqavwmx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mvvguupl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jvltwudy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ghvrhxsx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3oejzwmpz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lzulttpa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mgpyceff.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fcyafpno.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pvztuwzd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3wnnbaahi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fwdaxmtj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3olltydgz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3henvmkzt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3flcwseun.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hocnfbih.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lkwjharo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cjzvbpun.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qxozqdus.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qxrvystx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xckjpszp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3atcyoimj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3exusvufl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rkffcukc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jhmyngtp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bgtrkzwe.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rpvsxtet.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qukzbamd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3llaflenj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nrghdasg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ngrkjwpf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qheujqgc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3phimvfjn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kaazzqzu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zutoqmnq.html


<!-- 参考信息 -->