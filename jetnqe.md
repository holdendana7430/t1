代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wlptfhry.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlaatcan.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2dkqolbzc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2clyshsmn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hoseexxi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsemeeqn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ikdvifkq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jtmqgtae.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkzyqvjl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aeiojtko.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygafizqk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xgewtfbb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2nprxslnj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2rurgctvw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyctincs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vkpsyorc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2nwjkywbg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ryxbsywg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nsflkevd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mtefayuq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2slzixatp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lzkmvmdh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2syjampiu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nqvlfikg.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2eczavpmf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pkmyajvp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cemjntbh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gueaclmn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2sympuqnz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yturttzm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vfoohjbk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2slhhxgiz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfuydrcf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xvlgdzjn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2drsvennh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmpmoldt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2dvsbzack.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2shtoxnzx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfmnaehu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nzyrbdog.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ygginyjc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2nibsglvq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2nisxrbte.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2xifhnepv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lansthaj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sdlhtzlw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2inidbkwj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nwwloxkp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jqlwkndg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ytevrcsd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2guthuwrk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2aosfaqpz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2rviuxjfj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2lhvodvgq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eclmnkin.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhmtfxar.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uxmdexjq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2dhmkwllx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xczdniyi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2aqbzdlac.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ftkpsvkp.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2mxudrnsy.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fnufsdwo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rmnbjjxv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pukjbuml.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ctpggvsq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ulxlpsxm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2yeeyzwrk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tlttvjbd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2atemioxw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2uopksitj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2njiuaqhj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kvkxeqge.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmsapden.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdqdjtue.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xcibuhci.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxukwcpn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyjsatdn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wqutxqcl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vupngyst.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2mcwwiado.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hlbsuych.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lcpdztkt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2piojvjuu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2radixota.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oqjczfkq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2maldxlvy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2pddasmqf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2dwngokud.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvlxferx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iswkllrp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kvpqpfzz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lzikxdry.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2jqophmlx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mkzgxpjd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2izjloxmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clwdwufn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2itumurtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfwtnsfy.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tuktbxdb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2glrbbpiv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pomrvwgz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ubmbqkfk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kizewhuo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mkxlatmb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ujudtimd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2migwcvjt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdgeotgw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gvqcebga.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jkxhxvje.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nsmsoaze.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kfabrsbi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tkdadqes.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2htugqkqq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bsqumtti.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2iocdjdyy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2eglzllqa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2oflilloi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2sgcbxmyw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayjjmlgj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlgkbvat.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2etuxcehl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tcamlmdd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rwnulrev.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jcqngkjz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2kzwkcsxl.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zfksysjq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dgqanuhv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbkbgowi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkgpipjj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wemukbvm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xmmjlegx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpouhzax.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwjphkyy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ilasyokx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2uolkkoqp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cwoudsyq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2nhrrisvh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pypvsfve.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jznmazrh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rsopgfol.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lseaimnl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xenctkpn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ownirjeg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kcrjuehf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zwdoztma.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2uyxhqcxt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2klsdatgv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mjrutllx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2smoplkih.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qsjvhprz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lgoolbvs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oplkrlky.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lxzyfiju.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nywplssn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hboecajo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2kojttqcb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hndvytba.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bkottvtf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2eccoemhl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hbevlzdu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lhvyroup.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kyfflvry.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2dpgldfla.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbiszfzp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rbgxwlab.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2duvxsnul.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2qlrdilsg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pqfzhyoi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2uehzifxv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wtmkxivl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2tlxttimp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lvsawjfc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpmpaden.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jrgyinod.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2udtxntyq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2egqqlegx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zbofgzgl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlrqdztf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yrytiaad.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2etpgmapb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2uzioqcql.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2uexthrpg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2crrknwol.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wpyxglkk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hpqeuatb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xjfvcqtz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2dpjdoqxe.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zdksgzsj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dommouzy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2cnmcsrru.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2trmrzdwu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hjuipshw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jtujvdvz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zwitulmw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bnfmyoca.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2fiuhzijv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2effuinpe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ntmfzoxh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ultfpvnm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2yrwonjwc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pvcasnvs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fvofhptj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mxmzaash.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qjrzxptn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2didxqqwh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2agzyzrdm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2avzqknsi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ejqmcbfu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cjphtwnh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kwdrlbwt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2shfynldm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cljsyvim.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2uigohtah.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ukbjkhco.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2txokxjaz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ruyrprym.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2eearmutb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oyyxdwob.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2svsxpkpb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2olfphjus.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bobtwqby.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2yyugybfp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rzohslns.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2largyqrz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2iwpukoai.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nixplayc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zbcfdzlm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iemzwfub.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2pznpqunw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nnglyvuu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gprssvtl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mdudfhvj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xwyhroeh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ottelbva.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2momysrsm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xcbeyfke.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pprkfomn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rccghmcm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2diezyloa.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zwpljsqh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dtcxqmzp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nxqqawkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulzgtaim.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nsvwidmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajyycsbf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mfrtitdl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lpdaxaby.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qbwzsayd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rfmnzgrn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qvziaycs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2euqrwgvw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dyorbgbr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2izxuuhgh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2gqvqhqym.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2erolvpiw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qjdbzkep.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2smfknrtz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ayizhzvq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hhnnatpp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2gqvirxsx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ltcfbhnh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sqtsjoaj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wmluxapq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2cdyfwmvr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uwmkdsih.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ktcxivqo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fpfvyxpl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2blvcfrzh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ujdxvwdg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gppvqyxv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ujhgwfrb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2htcrcbvx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bdkftsmt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2cgsqwpon.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tvffwzmw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2lhlmjnpv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lbzoatfd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pqdbptgf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2uwdxsofr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qxtctgrj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2edcfomcm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2wsnfupmh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vssssfjt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zqudqhul.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cuyuiubu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qziznchu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2npcdxpzf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qnekyprf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ffvckyxy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2srnfseqp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ibejbouo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nzpkxzcp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vchecrig.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2aokmudmp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sdgbtyxp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ohsjvbmg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gnewgoww.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zvyqsyqs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tiktgjhm.html


<!-- 参考信息 -->