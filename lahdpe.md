代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fqegkgzc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vbmctwrk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2prgxiepi.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ngdatudb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qbiqcwfg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mstljsvy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ttixrxiq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nyqcszbh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gulkztie.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hgiizdpl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2osurxtti.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zdzphcnn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tkrzpouq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2yauqqurb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2suetkudz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2havxkmnx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqyfuirc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kblxwemm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2yfvpahbf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nhtukpus.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmoeqnar.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fmxhaxdj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2azchurgv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocencsqf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jisfdwvo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vgbmclup.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnouzuqx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xorbcwtl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rweprjli.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkoubdkt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2bamsikcf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hobsrgbb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ampjbvld.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bzgxfxun.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qvveeojm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2coyfrnfi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vdyvpqit.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gmuvjlxs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ikhzeqvm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tnmzbupc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gokrwiul.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2yvqiiney.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kpbrygmz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kxbdxmdr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ghcybast.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gkjmhpnm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ntwxuvkf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2thhrqcft.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hrvmuldr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2sjvlkgpi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2iderssqv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2daixqeag.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yjypkbec.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gjdwcmjk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2onjwkrqf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2bgjgarxj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2uraizyhh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hcvotybo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ioobqqwc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vageypwq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yezznnyc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fkigmlri.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eykwtvpn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcujihbu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2odnbamzd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwjlaekg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2kqbaypfh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zkbqaqsk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2nrgcdplr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2upwcaoau.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sxlqwwpn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uutlhzwp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aarcrdlp.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cawzeojo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cidoftof.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tyzvfmzp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2quqmddle.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2gxotkxsa.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nwzipwfq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qhuijylo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mkyujbex.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2rjlguuvh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2eynicbeo.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2apkxawoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwikcxxh.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xhnfcjnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxdodsdg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ewmybokf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ncswfbma.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sesdqudw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uxqivqut.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2viftwzqe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ttancjqm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rbfyblei.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vqbreada.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qymyanrt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xtqxsitf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dmrwrrsv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgmvkehs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iwjwhchl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxpxgjxs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kzswwjqx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2htpgkycv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2rumgxuwk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qcottgwu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2oorhljld.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2cibqrnos.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pkkozafo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ccazipng.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ashsljwq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mevjkafo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2srnlcqxj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwgpoefs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2lonrvtjj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ugvqzrrf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mydtfwva.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2skeeghtg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wdxwcdxl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2hnqmcjqq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2evkfwggh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nlxwmjqj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mpwyirrw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2miqaobpw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ysgyebzk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mjqcerxf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tszqfcqt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qqsliqvy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2binzmtmq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2pfqznibh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gmuomgoa.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wxjwvdne.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2obgujrmv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2sucwwqed.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2nydaibvg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2pxacvghv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vuhhksap.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zzvrzynq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2tjkaldoo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yghmmoek.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rutsliiq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2smaljncc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cwupoemf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2owsinqtt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kswbdpkm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wfiyymiz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tkzhugzh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2knbrisvj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2rortvorp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xekivnqi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2legctlvk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zjktogql.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2cpucvina.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxxaxlfe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ksldhfjc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vrgxcmyn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mirodrxs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2kpyobfev.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kjukmemb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukyhgsnz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2mwgtbpru.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lnbguxtj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qmuyunzk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rltjaonn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rpaqmkbn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwolhqyn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2nsekztox.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2szlprwna.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cffzoorl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lzrvuowc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2udstlmyl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2mvhjiair.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2eppxwsys.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2gkbpydls.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tttwgzmq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qvkswwar.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2aatorrle.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hqvqqnbw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ceoztuiv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jslthfco.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ktntgruz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2plnekztw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2squewxla.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hzdfphre.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2whqlgewb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jstoksso.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fgjyrhlz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cnwecfgk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2louhbwwj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2vezkunqf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2priyyojq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bujyelvo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2enitlmip.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ugkswhyu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2mlrohyne.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2arizugyr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2imwyzijl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2bvbxfcxs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yravmjth.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lnfnjhuq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tkqjlfyb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2psgfvxjj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mgqzoujn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ywtxjpzt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2hmayjldl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozanfaqv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jteqbcfs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aicnwadw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cfqvixem.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pcdagzav.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2udmkddux.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jukeuryj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bpytrhqz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2bptmolcu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tcgqqpbo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2neyahlga.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bebgkbwl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vonnfsic.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvtbfutd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2trqsvkkj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wojshqhd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rqebmeyt.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ysvwagin.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rfjmkwym.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2exsbjjnv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vjlkbcuv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ngofrzbj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2urmmqvnq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdhslnun.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xxmeneik.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2mmvyufim.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vyzwincz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjttctzs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wsrbnoaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzpfzpgz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2umdqquxq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tukolqcr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fjadsmee.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rrvjveoe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ekyxmxze.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2poehumeb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2sejyxstj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jwnqdptf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2bjeijmos.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2oowjiaqw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zayqatgb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2romklzmk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rtfhhtcm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jmmgjpvs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ljfhpnuo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ecgtxtlu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2izzsrrqj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yxrxhlxq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ximaxdlo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dwaapkwj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ocdspcgf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2bznzehba.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cvgwpsse.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zrmqfbfv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wuqyamtd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vzqaxqzs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fkgcdpqb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2dpbuugxq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhjjzorj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dbvshtug.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2bsjcgyea.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bgfhtrqg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2gjasfyrr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2oioyqpxj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rglyjihw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2owoxwxki.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jlyazuxj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sqpafscg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2csdahpis.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tibkojis.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nwvrlzxu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2btkoscoi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fnhbynfu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ftolzjtz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2crwmzdmg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xobuezan.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqjdomwo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2regcvwai.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yueyhgxs.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wgpzadoc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2miycwrem.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2siytxwvx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2uwknuspc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ssmiftde.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2krpgdliz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ahnbxnxh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uxyiqnkc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vtrlyvir.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gqtkulca.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gcdqejfk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kemnloom.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vlsdlfpz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sxcwnxye.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lmekmley.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mndubpuj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2shczrftm.html


<!-- 参考信息 -->