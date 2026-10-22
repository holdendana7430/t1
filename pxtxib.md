代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrkqpnby.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pfjtuote.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ybhczdmp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qsutcpod.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vnmednex.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2dhofmknq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2sopuoplq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2lchthpyd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkufhumm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdcflfoq.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfdvejvm.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hutlqbco.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ruyeidkz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bzynyheh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yijtggvh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2misfmfvp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2usenvyzh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uoyvmgcg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tflriavy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mbtmqrcx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2resgvtjg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uvydpoqs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nyztchte.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jaksmtpa.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2vsycrxgc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2bbdngnps.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqdijjjx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpzyyzqo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihlazqem.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yidhgrgi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ifjjmioj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2oqbvjxuv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnpzmaup.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2tmmyvboh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fnlrqxhb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbxffqxk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qzvoaibv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wpbupljm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rmoljjri.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2jvcwgkna.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qhpcybiq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uythikhp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2epwnzpgn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qadavhnc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aornsgpg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pkupyaqd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xmmxprvb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ujmgapsn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tucvpkke.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kvgknnkh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fkdvhbgp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvqvjaxs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2rmlwzzoz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2luphlndo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zxghvqdm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fymntwmi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2shtojulp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ygyoktxr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nncfhonp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2gihpqetb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2qwdxsdvi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ykfkwuhk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qaravdbf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohqzsfif.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yborwsyq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ykmlaozw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2gakgzmuu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2omdyymgx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ygywxbtf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2phxbyeky.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ibzosoub.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tjrpbcul.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2urnxwkzn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qnxnouqc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jxcvghwi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzlpbfee.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vqjshdvp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndijxmfl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2tzrxbuhd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2tbadzhrw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2djcebjkn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sejakhlp.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rsskkftx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tfnackqx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lkyrbmvd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uklhmmfl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qmcmuoju.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2waupfbyc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mvnkijbe.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2uxklaqow.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mtoqvwsv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tqacunru.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dzfsjjzk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fyafkkbk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xqytwfwd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tcdzrbum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsllsosu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vymaijhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlxeestj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fllgfqnx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wpvealqt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wsuwyrbr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zgjgytji.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2atfsrmop.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yytuchee.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mnfuachn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gzdhfapf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2caotfsgt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2udaqvriv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jbpbxvmh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zwfncjuq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ktdswkrr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrkvmzhq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2xdvztxpj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ifbfscfo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2rmppvbkg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gnxbwedt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tuwgwcdq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zokwbjfk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2zitemkvt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zeewfoke.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2elfnbhvq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsavkkwd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2klypciij.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mrgisiyc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2spijkfbf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdykmqcj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qikokwmo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2kazlprwz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zheztudg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ptnrsvjf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2uehlxviu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ezacockn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vfvjadjj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ddrfemtg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2yxdsgupq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zjwfefia.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2yzkjzxwk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2szkcsghl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bfugfenp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fpmkvoes.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gzkgqqim.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jxryfrpa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2halcqxfh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ivaamesu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2nzyxmrvz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pirwyhnr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2evnehavw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dlbiytce.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2cvuxnapl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bopinmqv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2icmvleui.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qwzfibwp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2zblyrywx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2topqubda.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jskcxgcz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2cybsnugy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jdrgrecn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2uikbowfi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2aikzzrgm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2qqrucfcj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2eeimfzny.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gajqaszg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2esecejnf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyhvkymy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2habhovsn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sswibjza.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hrkhkwwf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2yxtfzfsl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2irijmlvy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tzxiyxgm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2mpkrlump.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ebrvfjtv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kfqkyflw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2itkrecxv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dqzzeeow.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mpejnqzw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mcsfzaeo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvxdwqpq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wrxjmprx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fvmvxjjb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xrpqtgtl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2cexmgsui.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wclidygg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yoiasdeb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pwhcqolj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2llhzygfk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jewdoezb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kuseccus.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dmtjgilh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2wspcktba.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tnbbirlo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bebgsuxm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2worzoovp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2sowobllh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2orbaukgt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ajxlxqwd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fpbpsstu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vyafwius.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2pewnxtst.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2brdjllhw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mjqpjawd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2trwjdmyg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2acxnsfen.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nslyikvl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xhiakazp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jnhrtipf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2unpdwvrj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lnqmbbdr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nquvfabq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2hnskrhsi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2urfkjkli.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qvbeurzo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vxfdrumo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jovphbmk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kacapmfy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2bixfthcq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rvfdfujq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ovfevolj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lodmdkfa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sidksyop.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pthvixck.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2amuxdnqx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2teovohbm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2oazutqob.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2awkhnoxm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2febsldyj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2owcjnsst.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jtkzwwdh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2flbplmpy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jxabproc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ehxpokzq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2hsdsfrlh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pglirqnn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nxevyedd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2obksaumq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2sznrdhzv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2faaonuwr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2plxadweg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kteqzahu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hqrofxpe.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zfkccelg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqlyltep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzcichca.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yomibgdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppjdxytb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iwuppahz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jmbumiuz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gzotcksb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vrjlxvqx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zhotvhcz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2mvasgsxz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tvvvanvy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2evxcatxx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qeraifla.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2njptpgct.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yhgmpebq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jvroflus.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sisxwsfq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pulftsav.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qdxytqbi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gocxdyab.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nynlohzw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jomeutpg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hayxwecm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xaqybwkb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2alvmpgjv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jwsbtznt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tmwzmjxa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ygtwsfcl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lzdpyzsv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nxfluzps.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eifueedl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2npecdlvb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kftbodje.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xrucstno.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qmeozfvw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2raoohxbs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2bewimajz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dmcyohmt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2iexuqdnp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qydhyesp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2yhvdnfbb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xzegvvgq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ugisktue.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xnxlcxpz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lkftyjpr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2souukzkz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2axqtehlp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2adnzcxid.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ftwvxwhd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2palwiffk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uygzpfiw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2spbpxrch.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vnvzkcqi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2iclfbynz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2roumyoor.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xkpgeyut.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mmsxygtj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pyipepif.html


<!-- 参考信息 -->