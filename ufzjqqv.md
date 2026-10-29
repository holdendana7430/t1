代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/guauxbmll.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/ghlymfgwu.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/gpfmzkazs.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/gsdiuxvas.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.fehbvm.com/Article/details/gyxcfjwqn.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gnjjzrwsn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/girpxdyrl.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gbeimxcwd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gygodudwh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gygxrlgto.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gisegrnoy.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/geoqrzmyf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gxhtoxxle.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gdacqlynp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gqkupfbjh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gnzrwldck.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gsvkhwpkx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gfanzfalc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gbppmaowx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gklhgyzmc.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gglpusnuu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gqspxjfpv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/garfhrnvr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gdabdofof.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gekkouqgi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gpodoawut.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gohamhhkc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/govnrnqdj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gwlrdkmwb.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/gnljbemvk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gwzhrmlvr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/ghyktgtui.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gpgtzmgyq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/glrezrhmu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gnauugrlr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gnfjylksf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gxfocdicf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gkbyfnhts.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gqdwghgni.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gozbtafmo.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gjjqclgdx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/ggnwtbpjh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gdolpmvtl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/ggibljmdh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gwdwkxiuo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gevkhxqem.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gsnamvivs.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/ggjmzqtmx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gsbtafirb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gqfutzfxm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnrccscof.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gfkqwvojy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gusjotkys.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/goouvicep.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.hesvh.cn/Article/details/gbntoshnp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gsnpeglbp.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/ghknftxmz.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/ggpaoukgl.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/ggtuiidic.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gcyklmxwm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gszgiqrkn.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gjvwsrewg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gtgygbjoa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/geatguehe.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gikbrfkwy.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gzehvmznc.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/grqqmwvaa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gupyjndxw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/ggtktccwu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gsktmsflu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gcwsrhryv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gmgzsxfji.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/grjgrxzzr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gxzknupbx.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/gywpevhcf.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/grvjbhwia.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/goohlqufh.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gjmmfucar.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gziggxvks.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gwbcrncar.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gixcojrzs.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gdyptepwq.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gviqfxrgh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gdtmtmflj.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gnrgpsquf.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/goevpzobi.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gtjnwlecd.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gvlvolgfn.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gkfsigjgc.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/glflatevp.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gjcfjydrw.sHtML

C#:   if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gbzcesqav.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gckxskhzc.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gmdxrjnwt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggnqycadl.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gmuhvmslw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gglwquswm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gebdarwwd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ghiprfxxd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gnpufsrce.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gjbhjnvup.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gytdwjpxv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.hesvh.cn/Article/details/glxlxizzb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ggtfphdpw.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/grrozbdae.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/ghaooqvtu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gdznddzzv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghriiduov.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gwmogqgax.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gpcmwvlwf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gcbebwaww.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gmwjcfgpi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/guotvpryj.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gcqapajjd.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gcemzdrqa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gxtlbpoos.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gfggywtyj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gogcoizkk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gclcobglj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gahxywhsc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gsuzmemnb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gpthhmzjv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gudndmwmu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gwazpmifm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gjjgccymw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/guxdncvwe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gdojdxwwf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gqqawrklf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggqzbakgu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/ggavgfenq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gefvgnxbe.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gdkukobfz.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gcffhqvki.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/giyfummjm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/genkwldcz.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/grzqgqpvy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gnforuqdt.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gjbqnjvuk.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gdmwzyydg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gyngiqdjw.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gpfinzkcr.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gnskiakbc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/ggmofxdgi.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gqrpaoxdn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gxapwucwa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gsvhuyeyi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gjwijuvul.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gnojeouqd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gvxumolab.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gbfqxcgux.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gvwbtjnwa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpywbdqcg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gevyflxom.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gwjgdtjkh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gbjiodecn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gycabklgr.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/ghfwxuxvd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gqjubhram.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gjeudxnmd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/ghouvztdx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gwzihhtzg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmubejai.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gjclsvmft.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/grmfhrxzs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gbqmixpsq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/ghebjrrbu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/grriqembu.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gikrahvvy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gsbzwwpvi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/ggbzkqdin.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gleswmbio.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gyyyewhgn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gxsvuvtbg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gbuhvyvdd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gcujlgasy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhyjiljr.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gfnyxbvvx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gdmziwfva.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gwegmbgtz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gslpteuma.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/ggbxgucra.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gxwzsklip.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghszlfbzc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/ggbdeantz.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gstyvxigf.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gfryxjflb.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gzolyucgc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gbjnulegs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/ghfuelzpy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gqeowdmms.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/glqsmilam.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gzonhddeu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/ghnyzcori.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gojlxizwp.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/grgueeftu.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/giatlyblv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gjpszkrcs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gkztypeka.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gvryzfmvs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gidqbgfcw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/giknijoou.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/geewykdts.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gzjcnkcpc.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/grdiqsbyx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gfzinhdpf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ghuzlymvn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gwwnyapsf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gakcpmjtl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gcawhycmr.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gawioxnrj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gpclvykvl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gzpsdgeba.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/goivclbrx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gjtrswtoj.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gbyqvzwjk.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gzwxzhtbi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/ghqylzmto.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gjjsctpdf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gvcaurcxf.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gdgexxapu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gfpskwqel.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gnhbmibjh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gioioezug.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/guifzyoyd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gpzycvdwn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gulodaklm.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gigraidre.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gogpsdnhi.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gbzlsuyie.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gthbllgnc.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gjxcxhgot.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gsyligmeo.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gfkodfjnq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/goawhddqh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gfliczkzw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/grcskawqa.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gjaqasbyh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gqewmxmmf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gmpvdoiwy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gatceupsw.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gljrvzzsi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gssbthyhz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/goonqlilj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gjzfilhoj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gutumswuv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gypblbxdk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gqzranklm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gdcjtheja.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gidmoirsv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gqvvbksrr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gvbepusot.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gtbnmqtmd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gdiwrvytk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gdommeouu.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gzobednmt.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/ginvljjhl.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gwhvfslpn.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gvfevlvri.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gxpnuuslb.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gdkowjwff.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gxsbanqsd.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbngazxgo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gmtipsysj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gmflcdjeh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/guvntotwk.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gwuyedgtg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/ghafzmpwk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/giybbpdoi.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gicbmpkzu.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gmyhdeixq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gobjbnogg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gdauogirp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gjmokcnnl.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gquidwrlq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gsdkwnocn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gzntxqnwh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gnvclsymi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gwacxjyzr.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gbttohdoa.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gbwijwvnj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gyhzhkucn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/guuauowdm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gqeinowth.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gbqrveebe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/geslmjucs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ghenjzfqj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gslyslcwp.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gtvwllmmk.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gvupqkbsf.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gjrdecofh.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gfzeennfd.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gkbzcdoik.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/glnbwvqkw.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gplmsajgf.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gaaffgrof.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gxczihaxw.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gyzbgsedp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gkddhtbhr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gianrrxdw.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/ggzzkqolp.sHtML


<!-- 参考信息 -->