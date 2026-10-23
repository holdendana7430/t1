代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3qzdrwwbg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3teevjpwl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mlbxlnad.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpbexhos.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3woetbrtj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fykikklr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3psjxnmvq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zlxwptgq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wnwcksaz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3elfzlrcr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3cuvbjecg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3tlvtmpyq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3smzfkths.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kneulcjw.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqacmdyk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gojvjygt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3dwfzscah.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fwakasje.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3thpdmodj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3zleukahy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3irwnxjar.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dbayweht.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kmcfybdt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qxluiydi.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dkwoadjd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rvxngnjm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3nzubcknu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cuivsqev.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3evhbcgux.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fmekneum.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qvxaumuo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tafsobny.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ldadgwnd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lydpvqvo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3iuevfylc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3jtjsmmfy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryaouomv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3sbpsdxxz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3cxhvsnvu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rvynmanj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vkclxxzg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yxdxeqlu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3muvuakqy.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zoasbidn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3yhxgvcqr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vruqhbkw.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zyilhbap.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pfuunuyv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hgkvajgh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lqsctjco.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cvcjeryk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hntgtuuo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3chjetsns.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3mhfmhdgx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qxnpiqch.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lytmvwla.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wifdyfak.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hqjqmabw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qgxrvlnc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3awswzbse.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xtasvgzo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3abvrdosz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3dtycljie.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3druzeiab.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3bpdzmqtm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wytxpydt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ydoxcrwv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grkjvpoa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mwikldje.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pdzvfzik.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3nwoolbyo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3pjyclsiz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zpdqvqwp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3yexwpyxv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3tnhbifox.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xxmptgvm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fdzbekln.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfpcznqa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3janozmbg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubilylzo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jkxldqce.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jttvntji.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3djvlersz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jfljohzp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3lvwenuxc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3voqeddld.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vdhxuwwt.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nwnznxds.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oipccrck.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bhjfwbpl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nujebxrn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oxnldcbw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kskfawif.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3demurwry.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vwxaebla.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iluzfsei.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3oruipeqk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fafwsedo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3kqdqwsab.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ydhlifwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmsevich.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xnomlvua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyxtzqqs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wkwgkwjb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mflvfgxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrhvajza.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3agyeexid.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsesdhyd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3leqpbvhr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qecdzkhi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fowwpktw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nkyhqlqo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cslgdxhs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3nqvnvwod.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wlzuaeha.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsfhihfw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzarxyfj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cstiqmeb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgyfzzbx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gjvdncfh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zawdbmih.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bfwnfbah.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3rezyrfpz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3crrggwbi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3knvnmbge.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ybqfuqvp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbvnworu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3tovtyacf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ilmrarmr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xytouzaj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3jemgmywi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qeuyjotc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qygmscoj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3trwpyvas.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fcvzcfxo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hmnqsrqu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3dqulzhwk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3olfqshqv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvqdpxzy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kihlgvxd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vpppvkrk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pycijqwo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3soervywx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3siuinhlz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3yxcwthyq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lmdjxhdc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ajdgblqg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3olpzocyf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bbvpmjmr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3fvgzyoqw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3dlsrkyrp.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jhcmhela.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3auxwzxup.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3zlkkyvmx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gnzbissp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mwtotmxq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ihiwrfxj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kgustybs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3smsjeylo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3drxbtyvg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qdplwcpd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ucsxufuo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3dadtzwqj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qrvqwglp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3pbdphend.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mhejuenl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xnesrfvp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fodpbcbu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzczvbks.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hziiolwh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3frbtbolu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3viseoxah.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3bintoiwp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3uayavfzg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcfssmgd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tyuinksw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pcwjhdmn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qsosysrz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kcrkkrdd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fsulvhqm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3loxxqofp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qzxeetwq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqrlhldx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3viezgemf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3yjptwbyt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3urmfbtdq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ezxrvfzp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ftyoysux.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mdopgtly.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mnkxczdg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jxojbqfa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3moxzixva.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3epxlokus.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3sntjnmsi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rwsynbmg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3weuktref.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fttjkpiq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vuctfoss.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3vpdqjygq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3uzjxfstr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ohndnqch.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3keljbedc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3lhukexck.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ivdnjkcx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3qsqbamdu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xhemgmwq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ulwxpsrl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fbyqeicu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hlawbvzz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3abwlewxb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3hvwbcqyw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dwuiiszr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3nqsuytmh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwipyksu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3sgxhzcsq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zulykbkc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhdjczxe.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ghgpextb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mqvwkakt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ssfkxxgc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3lxwttaut.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rufdllat.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zdbskcbr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zaltutay.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfaeqqvl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wmpfzwax.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qtyrkcmi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ikwwsxim.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vjjwywpg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ifwfkcib.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3fetkkpma.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hcbegfbd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajvfzoeh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxzwmffc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cghffpib.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fnhwfsay.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tagkomgu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xwszllml.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yqreyepk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3trtkyoxu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3kialogwm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3yhncwfgt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nvyynaxv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkuduzaz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zksaqjkn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3giwbbshk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rrxsxvcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivtzjscn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sudgfilt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yutdjffj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jdoxfcyy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3iefqrkng.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wljuawoe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zoabwamz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3expzuvzu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jceagmxo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ceknibge.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pgnbcgxn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3igypbtez.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kakmzjub.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3xdcpjbgb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3eivrowqe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rntuxrxh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3snezbrep.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yfcpqlev.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hqwuzxzw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nkatissk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mluelukx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qvqbhktq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gaswhiil.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3upczfkhc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qmolumjk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pslkefst.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uobeidll.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vaswpymt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ruaoeucb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3phbazdrl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3chrcphdy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3gfyqvllo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cohdkkel.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mwpzlqft.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3smckvive.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wkogiiri.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pgjepcir.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3crfdotyb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vmstypie.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hpytvmli.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jhepuzpe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zshshqbh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3howtsegk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3siwkjgzq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xqkoezdh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jwyqgdnz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vtitriip.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wjfplils.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ujwgieqv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbvjqrym.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hebjwtaq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qqysgjpe.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3exsbjacz.html


<!-- 参考信息 -->