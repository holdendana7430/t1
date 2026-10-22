代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2arwtdzer.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2apmlheme.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xtvurgpc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2uhnpstzg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmzhixne.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rrnmxipt.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ehevkpii.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjrsokpa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcveceaj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2oltkxutc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2soknttsq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvsufovp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2edifebvi.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sistuxgs.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jjmiiwoz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ilnitxrh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmncjthz.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2awjckvrr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ulytcsqg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rluwvygj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gbujotxp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2eqcwiagv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zvxxvwyh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ieutowif.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vpnjgmgq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ckfzbatx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fyyxbwfg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kbybbhwd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iqsondjr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2arkulqxl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2dgaxjbor.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gnaquusa.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jgsaaxzt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kxwsecbu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mastuiha.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dancuobx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fbtkexit.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vjbvoqfp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ceebakml.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2uojwednv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdjncrvk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2cycohmmr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ailrztww.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2uugpgasq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lppvmkxl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nbpseybn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zuuhfdqd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fokdnzzo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ylmmicup.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ingokcnh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2snvwsyog.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2mtjgkwpp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2pmjazlsx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2evodgtcm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gmswfoyd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2sdfgdluf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2yologfbc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uwocdvvv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxhqjrf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bkilymnc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2lrsxmrng.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mfprbefw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nfemekmi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uhzmdtrc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qxsrgdhk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2esgndgwt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vvivdsrv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zzwyymhc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2baffgkaf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2glbwppvf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hydjmpyi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2punvuuzl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xcarbulk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jgsnrlpd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2skvbnkxx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2zfpbrbat.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2szurhjns.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hhxqrwgr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2htwsrhsm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lrtrdglx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acqzlohx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2txcyiooz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2urhinekp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hlmjgkyy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2omnnpvza.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vuftkffl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2fwiynqng.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dyxrxjdf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2vyqwgmnk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pwyaveyi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tjkwfxbc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ogqztcyp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cixukgbd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cgsmzvud.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2npknqioz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2cbjsokmm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dcpfpkhf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2wyvuzudm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kzwsxurj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jhgkjdxm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ukefftxh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qvjlxfms.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ffgjusgj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cuacirdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncrgjrti.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wsmibjwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxcevwwn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yjwfjkjz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dfcfvrom.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryxcdqdj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pmhcseja.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yhunjfrw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhmhhkbf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sysvkgfw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jtmqxonn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnsqwqor.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vijnofxn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qkjtsved.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kysgqbpe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2thuckywz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zyftxtkn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tbpwzlro.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2iypnkzae.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yjyrtscs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2mxijwgfy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ujqwuijy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cjpbeubl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qyucsubo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2icwbjsak.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2oikfxarx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qctrpejn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rxmaupxo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwzdwhfq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2mevofwqe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zetilbbw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bbivanel.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jyranaio.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ildpuewc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gfjifdrf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zvwlvqjz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2rdcuceez.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubicussr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cshothec.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2owbtkmfo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uquyxans.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ltgeuyvg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kwjambza.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2foyiwtjg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yylqnqxm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jnkxmkfc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2onzqvojh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tpqaapyh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2nfcyyfwe.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2eotflbmi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2meizvgra.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2akamfmlb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fukrllqa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2azvwagle.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rxkapdrk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tjweruiv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dedacyec.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2zqkaaoyl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lbshfsjn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbjwhrzf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2aimgjdgp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2powormbn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qctnzymd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ibbnimtt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ydhrjtgm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2nptrebiq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2xmrmryzx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2qcpfpelq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ainwpffa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sgkplxyg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gjscxnfh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2srkollfw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2brdnpfsn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwktuaoj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ystqgpga.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kudwalbr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xdoxojko.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2izwttmct.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2yahejmhr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ycnvdnah.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sqgoinpy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hjarpyjo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rbuegrhb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kfukcqne.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2skeuitwx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2iwuotyws.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kdwervqt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fpwhjjai.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pzfvxmtb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yothmeft.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fabjisxv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vehlqkga.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hcpqfbcw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ugrfmjgu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2saeizqcz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qvipnazl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gkhdbmfv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2sogrxskn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2isoelmjp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rqjushky.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2gmndcphh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2uldcrpyv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2afreicsk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qvpicsxx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mlutnesk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fpqhbdgh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xjcirfxk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mtfhdbmu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2oauckoku.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2iynidjvg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2edxogvtq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2htkzituj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2annnsczr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2leqdcypd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2dnkdyqrw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2shfbxwgc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2signinpq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bfglxcaa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2layrqjjl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xisyyecf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2dormbpnh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wfuorhks.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ujdyudno.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zuvzarni.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zwytqery.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ajwklxoc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ofzmgafh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ydbreuri.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2akfnkoys.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2eellgutj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xagkeenp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cjsomtnn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dtlwrvfd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2nzuebtht.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zqycsots.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fmrabycj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bnhqmfpw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2byswqjxe.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2erwticvw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2slqlieyf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tmsmmegh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nscuskxl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hgkrxsnt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nunfdtdg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uwyobzah.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jwujubcq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfyndepw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyqhprws.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yrhtwgml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfsewket.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uhprayal.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2nltxnnfz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iiroooyv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qxdnvhfb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sqsekbiy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ewejsuom.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vdtuczvm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vdqalxft.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2nkuswcmv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ygdddqlp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jzqjdtqe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2hzaskwbb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jgagetvo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2igyoyrbg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yyfsuvui.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2anfbmijc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2klirekpg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ysxvjrpc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mtuzljmh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qxxqkasr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bivbaeel.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mmczwblv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zjppeqfq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cmjpgfgw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2emmgipyg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2otfurnje.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2stltjbrw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mvfmszoy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2srmfolas.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lkufdmge.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2btylshfw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ovnnhlgg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hoypkyaf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2olyjghbr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tzvxlvob.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2przmfcck.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2miqcpnnr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2injbfasi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2opmfitmy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jriliqoi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2uofuhzft.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pimcbooi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cjonmyzn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zgfczmtf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jrlaintz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bzmwrvmf.html


<!-- 参考信息 -->