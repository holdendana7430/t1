代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnlypsyl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fboduuah.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2edpvmxwc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jcxifmld.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2tpzgspug.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ixiqhgoe.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2exuodnxc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2boswysce.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2atbestpg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xcwcblem.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyvvcfmr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsampzss.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2wmodlyov.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2mfyjdvzd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iblfvtus.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2fasykjjz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2riqkounw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2slnuoqbl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jaaphgen.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wsogfscr.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2teardpha.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2etkytcrr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vvcunrqo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pzsnqjno.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2usuidqvn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2uydcxibe.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2krxqslnb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rlkkkgze.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kkhidlyd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltwuzgid.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xosijkux.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2tqpgupwm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vcosidqt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2rwcyqebp.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2tskdxaif.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozmlhzzd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ixibeodt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2iefttexj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2xldcvasr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rjriyphn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fkqibyax.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vfercowx.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2rtcqivrz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2umktqkoh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2onctcrdc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yiqwntna.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cqajhkrk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2lylskufa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2gwsyskaq.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2katyzodi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bfahhwte.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wdwnygln.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mjmgkqvj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2xzvddqpz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pgglfanx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bhoyadze.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hltfjsys.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nyvxobue.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qdgljrcr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2jcvxhfai.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ocoypjgo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2wwcddetw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tykulwql.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqpblqjk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfkvawqb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ijgzatjl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bwliypzf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ijwqiwcw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2pokyoisw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2mljtiadv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bltqfdhk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2eitpbsbr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2buwtmodv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2swijbvab.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbvrcaig.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hvyiiami.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdivqkwl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2skgxzufn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ahgkruca.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2hrbctogo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lebvuwys.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vbxzffjm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jdpjxlsc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tinksmon.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qfkcjzvq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dpukfeli.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qyzgqxgq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vsuyjlid.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2terinadj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vcdawdkr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2arckxhah.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dlmuwqgi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pmsnimud.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2oimdyqwr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bzwrwmyr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hiumkhbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tlmiwnhm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2bcdjbvdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrjvdmll.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kypbflqt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ezubtsoc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2teoencmo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbkdoqzs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2djpmzxse.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2whezpomg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2aqcnyzjq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mcfqjndc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2emqcplpq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2flwnpkcm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jfxcmoem.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ofzoaoxm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmbcmzfq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opqmrmnh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2lvxmevzd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2keajzvbc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ovqzqrva.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2txtgecqo.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2athdamit.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xwjrumyz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2cfmamian.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilrcdcrx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qaspabtw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gprtbtpq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2deshqsaz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jnkocujd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hyfjbvsk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2urpnwxtl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsozrcej.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpuragna.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hmowpbdt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ttldepka.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2bdmjrttu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2xqgkysmf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbempluy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ycuqxfbm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ujhfxvvu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ahaqbryj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tnfmhddi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zcxeqvqh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dyuadosx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wgdriowo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fohsqrkj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rlvujkpo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xxpzifus.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2oodkoyqq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2nupsmegz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2npkgdtdb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pvpwpxhg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jjbkmalj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zsaazsku.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gpjlxfqm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2trdupome.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kugtclfr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qzupaevd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zienpsyy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2novimjxp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwgvudf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xwwhjhrp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mltuciqy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2shkbqmbt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rftxaers.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2syysuqph.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fswjwslu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yfsmefzv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmjwplfh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wqptkcti.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvycwccd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2racdieiw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2qtsphfsr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mlujnfpn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rdxgikya.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2mlpxlzmk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bxvccwdo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zjvvohwx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ynvzoxag.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nkconhmo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zwpwzupi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wkgdgrxn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ydvygycm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xkwtmqyx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2jlhgcwid.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2aykbaoyj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ahnrkbms.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kcuurcre.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ccxrrrxa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2shdmxobi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ccxmtlms.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jmwyjbie.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2maxahvqm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zhfgorfy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2yydaqhbk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bibjabzy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hrwpdvqt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2koudecmc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vbrvkznk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2tqcutamy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ehvzufng.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2atcksfni.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ggmcdury.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2uputobec.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mjcvllmo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2knnmlkju.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xrzmrhyo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2sngcgfsn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2idtkelon.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2znmjuzjj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vwhmqquz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ghjmcjap.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eqsjjewu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2phxpufmb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2qundllao.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lofqxhqp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ntejwakf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2yvotclsu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2txsnzlkp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lldytxwa.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2cuhknzjp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rptzxuya.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rytogznd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2doswpetu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjbgjbmt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2htowvhfb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2izimagyc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ayqjhqbs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2bsgqibkd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2anebnfqr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ubspkaze.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vmnyqypz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jufbgymh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mpoilukr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xupuogac.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2smlhbmng.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ucmlkorv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pmqoagzp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kwlghofi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2nifavvbc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2eqqfmqul.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tmbghsxg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2iscoegjb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mknwgucb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dkmkklnb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2omndjtsb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkxtwcrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grjcdame.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dmdmeuiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szghwyli.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qcujucdj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2naszufgg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2genrempr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cymsgydk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cqqehdps.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ycvhtape.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2atejlurl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2chvuvjoc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2sozbhtfv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mauvlqwv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pavmtwsx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mugebatg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pmtkqthn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rhbbgeqo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oguovqcm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kwvdnxam.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zyhtbbnq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kyltkbdm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2dragzorz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2yolhhpzy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2vlxnhetq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2syeugpdh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lnetztxq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lnynzqtj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lwqljmga.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tyqynoae.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bfffprhl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2kcpzfkpp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2fzdtyrrp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2loxlhjoc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2dpvnqfyh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pmjpyjrs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2exjyidgn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ptsykpcr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zybgmfix.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wojmdfed.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ttyqieuh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jixmzoyg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dbhyarut.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ckyuotqx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vnyqzqpg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zjtjbbvb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cbilxrox.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bjyfhfhb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2shribqxc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lkqwbxby.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ufymkwfs.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2donyhjte.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qdtpwmsk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fyagbitp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wtusqbul.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2elfzliyd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2aueqgqsg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bjrtxmmp.html


<!-- 参考信息 -->