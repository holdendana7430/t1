代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2khajsebr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2smygcqvs.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zruoqnfq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qhrjshqo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2jvhgmxcb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2gvcssocw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iqcjsmjq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2rwgilogz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2grmzxxhk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lzwystao.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ybvyxscx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2znduntnv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dtgtxben.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kagwfthh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rdfyilsu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sawmactf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kujufpza.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2rqxsyszx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2otvkfenb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2emgspfjr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2spykulgo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dkdtgvob.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zmhtiufe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hnnrulkb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sizrmcyy.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hcvaxxru.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2whbzgyow.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwwjqeu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2pqenayad.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gvksznwy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2apthiuls.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2inokajvr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2pslgidtw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cspxlfdb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qucvmfxy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2binaxzqp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ddfymnfx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yuguseri.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ubycxkpr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vjboudju.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ekimqvfs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2deqpjjhv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2crvolijl.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykxljzwb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hylgobdo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2psekswjh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kanxhzxx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tcuuvsmz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qytxyrit.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2stsmnhzt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rkigziaf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vbqouiri.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xfrajuzm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2rbezkjib.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2nvbuglzx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftnflfaj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kyopoass.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zawivrhv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2bfsibqoy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lpqofxen.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dryqkobm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2nkrpknsb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2lltfmhva.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nhxzzlqx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dmbzvnjm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fbgxpoir.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvnzdkgc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2swnyokvf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjicrxri.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ncgsbrbo.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2krwtwxqt.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qlyorcbj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2bentozfk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cwbzluok.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ahbsheov.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lowxwkyr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nmzbwcqc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zffsdffg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zwvyifvu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fpxfckgw.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mvrkakmn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2dhpwwhyg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rmoabbob.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bpiccuuq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uksjhvle.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2odwjgaih.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2luxsnrua.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ielbsvyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzdljmbk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2isbutqjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdafjymm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xvfegdvc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eofhknmo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2furbofgu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkftkmwx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zoxepymo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aynztzhu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qpyijaxg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nzksvgkw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wxuioexi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2urtcnylg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2diwhliuw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zxrjcodu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bklxcjrb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2elucpiin.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cytiqpex.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ioiknvtd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2uikhqjbw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2sqrrngor.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2lqvhaufs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2tntybybf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqfqgtpn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xztlbkwn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahguhqwl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjfoqiex.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2pxwvdskq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2cujkhpwz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xlmctgkm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hkijvshh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pwsrgukt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2naqwvnrb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2onxkjfga.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vvuohcvv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jbdlazyc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2enmsyduq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzarfnhp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kucjqzjt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dnqqshmc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fummoyqf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ynbfyphs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ddswhtci.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gexltrfs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pcxwtatv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2phsuirzx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ruhbaock.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kfgxicdv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jzvwjwzu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ufoiqvpd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2banakkpo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oewccxnz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jfrvufst.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wnwyduzc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ndrdtyws.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2eslrjfju.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ezszpfeu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dmaiwelk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2annieljy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gbwxtoaz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2odggpoiv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2idmablhs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nilbbevd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2olplyden.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qydldcbn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2nzrkpupv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fmdfqozz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ukrsdqxb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2othrneog.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yoklodvn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uriaibwj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2urkknrna.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ejyacdys.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2osydvanu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrspnahw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lssmotlk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwrsjuwa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckkgumlp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fnnqncew.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ucdhtmtx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfiwkjpl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2twfiiaqh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkglihej.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ydcosxls.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lcqrymhz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2filrrkng.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2lvfhwabf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pvevlfiu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lczywzyy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dgjmqgsq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2whbhbhib.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2nvvqtfpa.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2joydrzvt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2gittchkt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ihktzwik.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ivapewkq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wusmrger.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2uisgyuho.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xockfqle.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rrxpfnrs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bujfkuwo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vamnzcsh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xruaizqc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qeyjunua.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gfweruie.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gvssbwec.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2diijqult.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2cnsphwvd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gmnqnuxe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2voudeuql.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2syslkvkt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lifxmvrr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2wgffzagi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ewhlweqx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2cnuknpjs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2atxukeoy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hswdfdhd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bkubqimi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wozqclnv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2bljxaibk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xwzvqshl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ctovvpvc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ykjojykn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jomxmgjl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jckuuxzx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hadlvagy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sgfnfqyf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bmyjnjln.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2uoptteuo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2weidbsxg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2pmmvinwf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fokcqnuw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ciqagiid.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kunwsuea.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2clsrxfzr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ieriempf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2uuuubdzv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2qtpuiylf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2gsoywfja.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2efaigcpg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bopjzhic.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2owweklex.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2qrgzeuxv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fusqosvg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rlsrpnhz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wpioljxr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2gzkzyctt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjhoysda.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ifsccjqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hchcdvhq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gezkagjc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2opoomssh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2uoyoinit.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vccewvgo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2scwqvgfb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vkoxpino.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rkvnzgkg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zjtffiwn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xpdahuzj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zwatdsip.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nicwdrkl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oahjhhqp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dhkragwa.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2boxopcfa.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2gltjgjxh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ttqlecvd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzipghv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ldumqrvp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2esnjafqv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yqkigpkj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2aaicnobp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2cwkttlcp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iszyudny.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kjhewlmb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mdwdbhxf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xuxrgcsw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dyknsoxg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xmxxgfyt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rughfjka.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rljxjdio.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ywmffcby.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pbcsokeq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uyustslj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2fbxnhkok.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ovfvoobi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ajrcoqeh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qnvqxkws.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pluvojwf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mcozdrum.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oivxltwy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nlvckzdb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2lspndipo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2brnbzgxb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aqrxeefr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fplcjgpk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gylrhdjt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eihkqdlm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vmwjfmbv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2twbcsshx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rkeyubts.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2utgjnlxj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jqlrsyfy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jopjkquv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sjoixqoo.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2boizddue.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ucqnoypc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xyjamdzc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2suknuvil.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jvgnfifz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gcotlihp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2iqdxsvsw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2spibwzhv.html


<!-- 参考信息 -->