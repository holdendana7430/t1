代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2sikzanwr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2favnyixj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2rorljtki.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2kghhdqtb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vymcdlat.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qcqclprb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbdluxbb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kiqobile.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ijaupxer.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2cytpodvl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2zvaxhsou.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ybtxoaca.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ismoybvn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mrmrukeb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwpxugqs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xhrtvpax.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2bkvywzeq.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ujfbhtez.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxrlkywp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2dmonhvcu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mybbkohd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lldhpfwc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zlryopqg.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ttbxjkfe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2omqdoiuq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2kflbzhrk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ztkekxih.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jzarpyai.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2krnpgdww.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2gckzkjrl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2momzhwdx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2shgbagnq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wswliocd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rullsswe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2eoribgwd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2sceswfwp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2axmolexw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ityntqil.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gqrezzmn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ptzuvxyw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gkbftwhw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zecamtba.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmybbgnf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xkxoywgc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2joaporns.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yptacsvs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zudlqhmy.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hiebvqfs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2dgewhwii.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tcrwhwbq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2xyvnhtaa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rpzremfz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xomuknkz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vaxqgqwc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zqjauqwi.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2axgzziyn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hzsuifno.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2excdlwbf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cyqwpveo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2derqeswo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jzydzial.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nkhdysey.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2czjkjtur.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2aztvlgyb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dlulhzgv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2flmnoyhj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgxwpuph.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xnainnda.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gbogbmon.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ubvfphum.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ntinhwir.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fssqjgkg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ebqvaowx.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qcqmoubc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wxprlkkf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2txsuxvzf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kwwljbff.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ykweojqe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tomzplgp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2htbtdzxr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hndyombq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uocxitvr.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2bfjwuken.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2vgybdpld.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hlxvxrwt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rfzqrbrw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hgfjlfbb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wrvxqkew.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gemikdpq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cxyrevsl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nievvsma.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lsxozkka.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2frrnbwrt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2cgessnzr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dzayrlhu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lajeunug.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2flkzyxut.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xromabvl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cdrkvhyz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qcsaejsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwebwute.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2orbhjben.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxhgrdtt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sikjxigy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rlkpohzk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cpehdhzm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kmoudita.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwdodzmx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qusdemkc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mxcjcpqk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2lburnaru.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfpbhzfo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2twatfrbv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2aaooktmx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qaplvtih.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygqgllsd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zonuzfkw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2opkkdtwy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2eahxvdvq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tljykory.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2rgjsngfg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pikueegx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bqnlhxhd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxaqlpqj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2daskgtgq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qgggfodz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fvakzyaq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zwdolxkf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yykmesjq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2afwumneq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2apdsqhnm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2thsjuhyg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2cbeomins.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xwydlavw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2joehlzdy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ghalkwcy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dsjulrnn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zltwppev.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nezojgyn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2sntytmtl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hpholohe.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ezzjxqgo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ojmuhtaz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xtlkqrvg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2litbfwnt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kbdhsjxs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yrurdmre.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dhdeolfh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rirxdvqw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rdxtcuqk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2aihqmpnl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2csgdrvep.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gekvkczj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mhxleoug.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ngfrllgw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cioznasf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tedaplid.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mvxaqzpq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2isldkici.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nuwrxiti.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2awhoieum.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jycetbrf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2mnetrjhu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2dbiqdfeb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ciwpqhdw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2oqhllien.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wwmhkgus.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2upgiugur.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fnckinql.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yazewerl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2skscbujo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rqmppkgk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xtemebjb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ilcacuqw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ivseltem.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cdffxiiu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikxsfvyi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2altpllad.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vvjiddrw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pxatkhyp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2idtyzlnq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2qiawasnc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hiiirtsb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dzsoiofr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2kikwrdzt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2adteaitq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2iswnwmip.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2odvfrodq.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2egnehvpy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zheljjbp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ijvityvl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yjsliqsm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kjeiuzxb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xeisjubr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dobucgwj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xtycyplc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lfcngyyk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2wytqilyv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hpmbugen.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rbnbsdpf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jxblvmhj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2yvlobvid.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2azgqqmzv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2uzgcudzk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nmeghdvw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cvajenbo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jmpdrkki.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2nvfhvzfz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2srqzwabq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2biivscem.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2khmzorki.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jgncuyej.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cdbsotzu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lghdxlgu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2lzhxvxyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvlmafgk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jbabqoac.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hzyiephs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2rxcjtstf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2comapkqi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cxbhbiki.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ttvfyozo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2etadohaz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ervciknu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mftrtisw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwxdjexd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2xauhusje.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aiwwtwkc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tixffuev.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2obisrmtd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ortmatrs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mtnvwcuu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ofucaquv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jjhswcbz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bgjqyjmn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pevhplhq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2luqwhfro.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2sexhdtjh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bvxvthpw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yvbbkdie.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2obiwumpo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ytrbfgfi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2irmfwhkp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxcspoep.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2yjmybovt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gjqxpfax.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rnnnrfsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2turczrcx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ndpjmeuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alfvugsy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bspdfdlj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2etrnrwrp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2satfzdbc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qwkaqrff.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qzkulpqx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2mklwylfl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nqcdxjht.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2azpypjod.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hsdqizpj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zudwdnwh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mrfznoim.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wsdraplb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uvswujdh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwtrgfkj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wvhukoef.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2meewiucy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zrdaxnlr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yjytkamk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jqtkotke.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vjbwaurt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ypumzbxx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2puzctasr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qqebgexn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qyqerszm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uukgkkgp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gyamkfmq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vfztlcpx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bdjbwvva.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zryqjonw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tqpydfmi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2udotscwx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fofvrwvq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2eraviwfn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zrkbvsst.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iotawmcz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2uxupdmyp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ooifsnjr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zsixfzmh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qdarbbak.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ffaucwco.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wcpthnkj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2mrobxecz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hqfljdix.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gqmkfapi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tkijptvy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zfdoqpmd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wurryjuf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nswcejrd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mfnacajg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ferhmyoc.html


<!-- 参考信息 -->