代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zegqozbw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2fdygewnm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2cdusflbl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjrytgif.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlvaqtrx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ordihhwx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2tbjgxjrk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2lfuvmdxw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rfacmcqg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijwwbvlg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rhzwjjqe.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2olydrhzz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhsazeld.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yolwxiip.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtsowvwe.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ukgqfbbq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2loyetgav.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2eaztfbgx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2utenvizb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ogadaqwv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wnrpsebe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hpneuqow.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kkhfatsk.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2iuwvooqe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2srjbanrc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2piogwzhy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2jlobsdgy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gbvellmd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2rqgfnucj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckiyoeum.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhnnjxr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jmqzelks.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2okdnrquj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lejcavaw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cjihryom.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ogtfcfzc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cbfttdku.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2lblpwgfq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2lommqggy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2udmrjhuf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2mcjebbvk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ldqlslek.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmjuansu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2zvydpfln.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ninedzui.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vipaghkf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tbwqycvu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vuobkspt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gpmxybjw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2rafqjvsk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2eqngkfjm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rhcipyfq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lgfavidl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wxoejjhn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gkmjydum.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qiozvdtg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2voqrrlfx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kuwwybbe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2clehwhup.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mdiqhfvs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2iebuidyd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qkhfigfq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bdmdpjqb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wwmabitv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fucuztoh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2iksspren.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgfacpav.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmpsodcx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sncrhouc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2tyqmvnkf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2sowbsrfr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pfpanxvt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2eerjazgp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ngsscokb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2sxowmgpz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lqbnpfne.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmoxpvep.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fuifzyrh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sfflsxjn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzxeucvn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tuocbdci.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kquksjtm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kgvbkmhz.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vzoofohw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wfdhftji.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cxitdjal.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lepetjrm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2itorgagw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wtzdbpdn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2smaetghi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kmhkaenu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bxgglzbe.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ynhvpmrk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwrthyan.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2frzoslov.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ztnwuyik.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cljxdyei.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yqxhkyhu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2iwbcnamm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zrjimgkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2orvvmkoz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nfkpebhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swgwbulp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ctbibmoi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wdxvmwbc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2edbybpcz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbmhcqgn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsyqnnzf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aijfrdyw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kiwtjaxf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nehtkofh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2szcewkvg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rzmdhvhu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2htzwuyre.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufypqinl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyvpvwno.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vqoaoclo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2dsqclcpx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ztzpbsrk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hmvylurv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2zonxpfwl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xozclctj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ktcnxffk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdrhxtev.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qksurzka.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yqaotjtm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2udwzwatn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qeciintw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yxbrnzfd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ucihbwuh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2oduatymw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2onhexclg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xjmghdng.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2voqopjpe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mdxqzesu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2odlxazta.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ghbfvuyo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2opbwwyji.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rozijcaj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2clgqysgu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2erudjjmt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2aqplcxjj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mivityrf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2acyjpryz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wkfeghpx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dxjiexhg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2dtnlofve.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2equngmon.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dfzfgdbx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ehzkuntd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nnasrpxd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fhlcwlvn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vektoppt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2garvunrz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2chzcaglp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2nvgytoeb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wvjzkerm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2wxotnftq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lthpybri.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bvdetcpz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hyaweuoy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lmkbcosp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tyiyfjwg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dcsipewi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2epaqfoam.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vutpllgl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2deeoiena.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2odzcrnlu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqswxrhh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2puvlotuq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fszrxuoe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2spyhumvl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2kibhpwcz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixdgtavl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcurahxk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vrzbpaaj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lazzwnvx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2usbyejcx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xgpdipvn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jqjcbmcy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gotfqsbc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2mmcyinly.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnztjogc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qhhisdyg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2neyijzjn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nhdpbgty.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hhgbbjzw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2efomwzwv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qecihiox.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xcaqvgxt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lckkhskl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mxflqsnr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2elwfmday.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2imyejayq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fzepfjmb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2tyskmkrw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mdbylmoq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2cfbcpchk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2owuveeng.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2thibzdvj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2erloboah.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2virbhlvj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2gyowfkil.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rumezjmr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ktmyfsum.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ffiaienh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ecyokdru.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bqtovpji.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zftscelw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2yttpuqap.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zmkckkyn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2byiqsitf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zltudcnh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfipwpqw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zaadzhta.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kdkhvvpe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvrndpnr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nnvpoweg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zqxxckhe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2liyclegf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mlyiflph.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mhrpoegv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ntpttwrk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dzkbwmje.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzhajfty.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxobqzvw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2plqglxsr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rvznrwtv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2jyumcddi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yenbagie.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2uelfnkqx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ckbfbvnl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddobwmfg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqocqixz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2utuhkevo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fzezfktv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2stldllfl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2sjoklrtj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2pgnjsmwp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xgayagtg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2kpeqbept.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2konpvjcy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2asdvkuza.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muqvvrhh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2umrigiue.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbfxpstg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xmpraicy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yldbofkp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dsorsgzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glmvzzmh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qlsnaavq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xjtpbbdm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xciybelu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tadgndrj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2tpcgceht.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nsvzdzrx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2wnsnudbx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vrcgjzep.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2wxqlotcd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wlxopbzu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2atmlgvac.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qyadvbth.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qjzofmwl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nxafyymc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2htzlzcyx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jvigmqad.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2bqeimgnw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2epxuqwyq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ayifyzfa.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eoubtvdl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rmlxamse.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2fomvniqn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2njrfgweq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eraxwybx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mbmevjza.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jkmmkrdm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rntvkijf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lvfkqdnl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vemttawm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2phsbfrww.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vhztusdo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tngrebfw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2hprwemvg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gqnjvxof.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2galtamjg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2npraaplb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2rktdsnka.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2idkalhxq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fhfofdme.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2orgwsugc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vmjxqakw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qnickvhb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sviewjoh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kmcvbmtc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pmlswnfx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bhpkxolx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yidsjtxi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dohsfejo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vfmszbyh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zbzkduti.html


<!-- 参考信息 -->