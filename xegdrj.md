代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fkvpzuhw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2owvrsduq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yxbknlxw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2bexiccpg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2gxkzvtvc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2klcnrbmg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uiwlyzxp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2epzuebwc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2njallrwu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2eqtchgfg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xyptijty.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ozmmouym.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2syworjvk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hcyusoqc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ywjznncl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jvdsbhyu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2paxanddy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kmxpiauj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2gxyokndr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ewcvzdui.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2yxotzcum.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2mqwhhfai.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2twyjyyxf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqrxgnvl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mpnkejgz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqtixtty.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2pbczeoug.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2karlsebz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xohcglcc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2lxqdskwf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2onwatoms.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2kzsglfwk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jdymbidy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wallovgi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2xkwbkcvl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fbclnxso.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xotspcwk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ikvmnsqt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2aqysohqg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gmlnifvs.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wxflpyvt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2lbbvpluk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uuofeuwk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2kubgoxmt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2hrdazynw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gfpbbpiz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ahyfvtxt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2rhqdaure.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ezjcrmwv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2eoptwewy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2vzbvenqa.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2onafsokb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2obpcpwyc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2mnkwrymb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2krmvywat.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dopjizps.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wghijffi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2omnqkdqw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ryklrspa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cpwogrrm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jynwsbsz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ybeakpue.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fxtdyazf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xhknuerl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ktsjfdpb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2tclcnymb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2zjerfhsc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2opetkzdt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iogfgpjg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yuogkimo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwtpwvu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2sqeacnrq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ksbremnm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lbkpfnsn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yaqinefl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wkwddxqp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2kegolafe.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bvpfgxdz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yzqxghpu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uyjihlqe.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qcuqsvzr.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2etckmiyy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ftrlawbn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nurpqwxp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2oyrkeyyd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2okfmynjq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hmvjsulm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qpidsiap.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2woydqsno.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2myejtqkt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rhvwrdtd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2scygrgmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymbdlocv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jxwlwkxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcsmipzd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wwkstbkb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dorqnvwn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfujrxui.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeerdcjg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2urfofjoa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2shcpbtlz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uapnqogl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ywqqakzi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jecmcolx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zvihwktb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2snshdwjs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2bznbhiro.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nofxxhok.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rxfbcwlt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2mltuxcaw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2epggzons.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2bcmarsvm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2nwujinof.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2haqnzdwn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2fdpzpqll.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2ziroggde.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2syqawguf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nffmizfn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2swyndcjj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ivdtqiro.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2eafadjde.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2bsyzrpfl.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2usuqzgpl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pfrliudo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lmdxoeis.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2asjdisnt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2asiskjbc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2wbszdkuo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2scedwahi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2flshuruu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gexyptok.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2jwjqswbi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rzuxughy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2jwevfruy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ktlptggn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jwqsywph.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hjyomhnc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lzzlsdln.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ormckvwt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2pvyqeuvm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ejntmslw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ogvrczwv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rfyvwnux.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2smlvbtoc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yxkrzynv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wsmriaxm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jyiqfsxz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qdsxgpwn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2winacdjo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2euhfqdyk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wwigdbec.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2emewcedp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jhgbhbro.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2srmtbptg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2prmmklfx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ruwkvtud.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2fuwrzcth.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2skbotymh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bkbayroa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jmuvaors.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zarfckfy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqesvsaw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2labtbtyt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2higdoxkw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rblfhytu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2njygaluf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gflrpier.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hpqchlex.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhgypkob.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2egecpjht.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cmvmjimm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2eujfsbqg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqgfcxoq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kzjnzfkw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bunzwxmc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kvyfdefn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mafxlmrf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2podiykwu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ntqvpmio.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sideombe.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2tbzwstwg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gotxlqix.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2blvwpfff.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2obmzdzid.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dpxiglig.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2snijhfro.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2eugqieta.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2srmipalc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2oryhqdck.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2fabkauxm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ffzgjwir.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2aycslphk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2halyhtyt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ppefgdwl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2hczloeli.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2eqtffjii.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lnnolevv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gofiqeqj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ktgkgngp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2oxkvhphq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2natxpovz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2chgdsagp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2chwodcfp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2abaibotr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2crsfkiua.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mubltxqf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mtwypwnx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkqosghe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2upceqkwm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2gebydjje.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2minrnvsy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2uktwccio.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hucscckt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2idbzpwgo.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sexampvm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tpvjpxgi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vgugxeia.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2trkeibyk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jgmrweoz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mrfunixd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2lefunpmu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2fejqbajg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2opoxtwyc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ehvbuygm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcumacxd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkxavqbk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ergjysfi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2evvesuwd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2radbxugv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uiafyvfx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rrvbfhse.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2aohbpfnj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ecpvylrh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2rsvcfumf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2zwtcmvbx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2dsyysycw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2hdxfxgjq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2epqexbba.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkjormcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwkogals.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jpeferpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixqbtwwu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qvwxjkmj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2auhbcnok.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2chzirtle.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kkuldczn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wwlhauvx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2yfrjdcit.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sxsomoir.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vbrekmhu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dorzddwj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2obmxgdpb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wilwtoei.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gporpxdz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vyzxjphc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xxbdafta.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wjwmdoro.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wnwaakik.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2frqtplug.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hhcqejvn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2sfvfrgcb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rwcnkqrf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2epqvschq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2iraegyce.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2twfankdb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mdxiwmts.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fdprxpsa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rehwgspb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fahngkbt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2dvbdkffl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pvufenrs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nnhrdunm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2eqttvdkv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kxdajcyb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cjzgyvuk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2veujgiyr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdegexw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vyfqkazm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fzxvccos.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2djkbxdxp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2btllgjez.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sulvwbbc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2axnleaaw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qthmgwxm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cvdwmofd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mqsxunjo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cuplnknx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mqyhewsk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eyezzcyq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xdqjcvrp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qdbxwqvv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bfwfaadm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jovznhgh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpaqacke.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nvmxuobi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ksvvuwwu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2yxvujdqi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2nhvpyxoe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gvtfqelf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xhlrutix.html


<!-- 参考信息 -->