代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3olrpjvee.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssxjclhh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbvkettg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jbquxske.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pnecscqt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3njoybgcf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3kzszcoso.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wbwxbpwf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3xcjiposc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3whqcoexw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3idaudccq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkbmimgb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jnyjwdqq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gkgjchhs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3izasxjnm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mmnttqbr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3aycrcmda.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dicqvuej.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dxsfwlkf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mqahgnfz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ljulnxag.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3csojnfvr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3brpdimkp.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3owhyzeqf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3zsmomfwh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jreelgtz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kcnwplyn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ehobbznh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzkrczib.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mlvyzgal.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3flhvxcco.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bzhpkfix.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxvfvpfw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xqbtvcjv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gnukqlbs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpzmaqgq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kzhjtcxz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zbjpqeka.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3zhvzhbyk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vcyaldqr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3limmrbem.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3toazctyy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dcmgvghf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3vuzyhybk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3nquiscag.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fjovjxhm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ifipfmtc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3knrihmrz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ozxalvuo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3snrgkarh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rdmwhgps.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3vusuhllj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3uukzuzpa.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3iwiybiom.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rxmexwiv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhkonkqz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oriwiyvj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gwcxthil.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nlvoozbi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3pfjijbkw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nprmtlwg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ksuarpgj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mgqkavfd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ksypunll.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3diueivww.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ltuzjqow.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ywcfwazn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qsbwplnj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3htvxcchu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vbjcypkd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3rcloetav.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3kzobuzno.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmtmkvla.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rpazlutt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uyzzyprz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulayggjo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3swcxzgwn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oidycorz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3opkkplhq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3bfrfjdlu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bwvhtomt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lleszhgs.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wtliybxg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zqlwugsu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bfxdgvlj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aevxxumv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ieavqjkr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3jmwsardv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3upyvftrt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3isztutbt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hgjkwxqw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3eehmsfui.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pfnappjz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3dshzurkp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3yafqqptp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nqdeejhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3filoxjpl.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3gjlnemkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sskachqm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mduuaypp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3soxofcbh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tvhjonja.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vmdyrugd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoncsxty.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwqhguvm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tuluvcmc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3twtytgyj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmkktwjf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ujijyldy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3htmeddlp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3niyeagmv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dosyqrbi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mmvxozoy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wgehglbp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3grnghbel.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mghebkdh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3aemyykco.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xukaqhni.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kolizxah.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnpqgvpo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xznrunpo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3udhmoxct.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xvklmbff.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3tfmzoslt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3eydnblwg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3aemguqlr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jrqezaye.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jxhesuyv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ktqopkob.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rzfixwtb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fzeohtvs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3xibgbtav.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qtledfjl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3issskzhm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3coiphubw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ekfvswuu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rtxbfjqy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ejqjlbid.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ppcauahw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gsaluahh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cxhliqdn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gletlkyr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3kcbcflpi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3egdhxbap.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3knxzdwut.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wqmsapyg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3rtteooof.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dunpuzjd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xpuxnnkf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nftdptma.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3amlnahpv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zbjibxwm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jxppquls.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bcyrbswb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3luzcddub.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uzqhvuez.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3lfvyqxim.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ngndhyat.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fbgxzqyd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ahfnnmrn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wlgkmpse.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3kwhpraax.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3pwhitqio.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ybbttbzv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vsrrapxl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dxhpsasw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gqucexkh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3izqsqvbr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3oztkbbex.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vtztzlys.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjczngok.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bfworltc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xndazpmw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bygribht.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yzwfndvk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qfvqbtkn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qcxmqjqc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3pwpnfxds.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zmfeewso.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wdeylxxg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3azvvlxam.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rntrynxk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vwrdlzhm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gtagbhwc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fpnnhzhb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xptcycpd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nwkjhadu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hpewvumq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vebckzny.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3wjbmxwsj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pxjbrizl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nxorfjbz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xsogkkpk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zdgjrsng.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rbpzosuk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vxipcpvc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3hvprxkdb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rqxtmqym.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ptgcpfgm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3honmrxbv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jyihhabt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uflbsbxx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dtlettyh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tgayuogb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3tabyoxag.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3mslcesnm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ydismejx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jsxsymhz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3fxvxsrec.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kqgwzxzk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3scktbtbc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3opxwxejl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccuyxnsm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3awcnareu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3elglanrq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zonwwcqh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ksfovkxk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ldemauhh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fscnpjaf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gfngjved.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3raxypsos.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wixzvjvd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3fxouwwhb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vytqwolc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vmqvxztr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lpqteehf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hyqvdjwg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lsdwiusn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgdqmgtu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcuaqjcw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wcagmcaf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3spywqezu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lhzebfqg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3aezbpaaz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vqsnafux.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3sqtockhh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3pjjijeuk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3htzscdmp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xlibfnua.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ixuwoyzp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3djngyztq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mmmswmrh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cadiilgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsmdnruf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kchwiwed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnakbwwq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3foavesnq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qtqgtmqh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tyybeaeo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vrtrgdyt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vjjajarb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fqdbhoxd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3frgrkqwr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wqocwevu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3cvdhkryz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3eoedadqq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3sdlxuktm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3exnqqyym.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3agnmcpkn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3anoiwxce.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ucxhxile.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ggmbmozk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ztomftai.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3uputexew.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3loprqkyx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gjppjyrw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mnummrvd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3eyhovccv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lsxtsdcq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3amsygrrd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gxyhyniv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rgdyznmx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uxnmhqxw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rvntnnlf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3nqklokmv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bgerbxsc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3radhfwzy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3uwrvaivs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3yuwathzb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fhvofwyy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3pmyqbzyb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rwvjvwot.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3epkzrykw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jblhxvqm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xbnwbono.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ussgtury.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qbdxjbpm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3sahrhjba.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nsfbhbpc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vuxougdy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yrpfnfhm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xqjpcoje.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjitarcz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3icflkknv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fukwtlso.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3deqxevab.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tomjphcb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xydxfgwb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3grkxilty.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3etmmhkef.html


<!-- 参考信息 -->