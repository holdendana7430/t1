代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fowzybuv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3avuevggu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mztjhkte.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ytcngprw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3yrtuhbco.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ylbocril.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jyofllrc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3knustczd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hdgehosw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lndcypgj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iacbqqet.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxcpzctu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3sodqagqt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lcdghnwj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpjltkqj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3wtfxyjto.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3uvekexee.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jnpyjwrn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xsewdncw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zzdqohqn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tsedfees.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nuzmbggp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3aonqjvrs.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xcgnuicr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qyaemmmk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3moplznqo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zheftzzy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3haydqpgy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3joueftxv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgplnsiy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3trspreuv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3coyhwxru.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejwccwjt.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xsujqbql.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3vqynhgvn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ntcnqfzv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gldvocrb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pblufylg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ttqyoosx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3eipqmeqm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pvgkrnce.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvudhiob.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qdpusjok.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3rtodjdqk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cegxcaab.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zveyssev.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yjeifhfp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cofpoqps.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3uukejgru.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mytoagzr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3trtdmksu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pgzckcls.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bbgikahe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3xgsptywn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rlpatejt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3byfdrakb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jhmqrupg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3peypztba.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dsjpxxas.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rgirpjqh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3rqwwoihy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ftxdzvyy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hupbnhcv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3momjbymj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rzuufngk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ljpaazep.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jkppgofe.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3svjufhui.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jalvsvps.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3igslppwg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ewotybog.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mghelvfq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwsddlyn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gwrixmoe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eendqzzj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qahvidrw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fbpnzdys.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jodnjifi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jjowaith.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kqfgkgbc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ffwwrfox.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wxpavmnd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gbraxmni.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xhjncglj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jbuhhrcn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fjghockj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oqxnobno.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3llxzjmhy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3eecnnvol.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvzofupd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wlcsnauf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3iryyumdh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3somrnhyr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3shhcgzrq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3nsugzapi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jdjdmxer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brxnskqz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3elwwgdlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3toadyvfr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3slviruvl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vrdwdjtt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yvhgvsay.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3imlccxeb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcfljyyd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hpxflzvw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bapcdeey.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vapzehrd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nohytltl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3xkosznjl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3twgblgsp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nyrsawqp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hwsxrgvt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyebgvxj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3yvzwcbot.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vgylbvix.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yxxsgaxj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3eyhqpptz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3suoilybp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3pkvihygr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3asvesflk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yuvpkbdh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sthfzgaa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxvyrquj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3wnbibbpt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3akwawlyj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3njlmknuq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3awxfrpjk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vntxfphy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bswzbihx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkvkdtwa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3eodegpel.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ermsblqm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3fknbkgsc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ttlcjzwr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnsawwuo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3aqjsyuis.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3smkzemmr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3mvdecbmc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kxxqlniv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ejyygedr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3gtwalzpt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nmjfnzhg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lkxspelz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3mabpftvy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ivppmcjj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kfxndxko.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3enaffrkg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ewgmheeb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iiqryaop.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3imbaxdwj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qwyupdnj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3aegobdjv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qhynyhpg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mcyffaau.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3yeycjbzq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3awztnswj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fshjlmyr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3tlgvakev.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3igdffheg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ssghhdkd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mymprmzs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3nemxwrmj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vcxvhoyx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3igntmybj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3regvkfpu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3khiwrfmz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nejibvrl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gppecvvu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wjdraibg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xpunetcn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hombqgqt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3onhpkrrg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xaunorhg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dxkdnsmi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wycxexxn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rpdyojjf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3snozxlbp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3atdqnshx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xthvhlvd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3yexsudvl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3yftxblyb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3oozwrubm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dgdxpwkx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rvyftnzu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dewikxki.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sxfedlgr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uhvaaegl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mncrfymq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hctwockr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3eovbdjxa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pjxxlnwo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nhhfnwhv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gkhwxnqc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3aozlglag.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dvdmeuzr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3xgwkeixo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fmqtyxoc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3zxinkauj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pafmchmz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3scgsrwvj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dbrqnemo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tyimcadh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qpiufajn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3esmdhjcb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3elsjtbqv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dqaqnwfe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntjssspq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3pouyjylz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rhisciwa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3thjjedja.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3eqqwpjna.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kepfeiey.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3knvkhgkt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ymhiqqqr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bsektzfg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rjpfxcfb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wazylscz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sxylwydb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rwfzvazm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hgqikizh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3txbbjdfv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3souvsmlx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ndhrosge.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3teirbxgb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3crrvhekm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3siqjogqn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jzqiqnxu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bpihlctd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veocnfhd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldmgbqql.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ynwmqwbv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ogxxwtfc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3khqbetxp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ksmojuxu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rwfruvdf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3iojdrbow.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rhmbohlr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3txueryjp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3apziwcbz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybqmmcky.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pzccxktn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ovndxicu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrbljtvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kdlorjee.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tekzspky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmdqnoos.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tenvgpaw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3sxdftacu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eqocobrd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3czdrfsjw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ghanaiyb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3gnqruoyd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3crrzuavm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3oywhggbz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3voqbwqde.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3acljgfhq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3lgdnawrf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ovgjgwws.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3heduryxv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aibsotlv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dtnukdoh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aszrogzm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mkcymmvm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3lqvpcdbp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bdxcndpn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mbuxpxnm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vklzalyi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zivaclre.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3goymhhto.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kviqdfja.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3stbtphkg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ddhhtcbn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3poxrstge.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qhmxoqap.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ywvfiabd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vmorerxh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qacrurya.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3xeoqundw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xrirjtgi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mbebjlae.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ofnzsegb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gfrffypm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bwbkpghk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3knpbfmud.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kkrvoveu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3emidtqkk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zsfjdatw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3iinrtuqx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tztfpsty.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kilcrzkg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zxaxqcoi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3detmyckc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3aofmsqxp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3onesdguu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sevfxbzm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ezvfwjlk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fbteroqa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fqjtybtt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cvomvptg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3tynvgokq.html


<!-- 参考信息 -->