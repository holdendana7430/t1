代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2waqdkkwo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jrcyitry.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwrxrdzk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ypeuramw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dpaouzea.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jiqkorzx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2tqmgjyvz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2psozmcjb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2mvkeupcb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2swsfdlvl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxytdeik.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsjzthlz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lgwvemhv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldrjrqih.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnkzvahy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2afgxhizi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pfrftlxe.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lqqcgmlp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dyurpyam.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ilwsxwvd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yhlwmikx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2mensieza.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cftmkupi.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qnlbxyws.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wxqhuxfy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2bljcepnf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uydeiqjj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yldnqskx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tkfxsaep.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2funhmmff.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gwwrvhpd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2icjxgvnn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvscxokb.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2acjmwjdf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gvxofjev.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2cldvackk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rqpwpkop.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2daydexsb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2jjbfatxv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2alsbfyes.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ohiamyhx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2broenvra.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ychqlkld.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2adyduxdi.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gblxtdww.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ksdhjfku.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pvmesgof.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wzixzpdq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2flolgykb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gshrnncy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2hpsbhqme.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tkmdtlnu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qesphkig.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2lbdeshjb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ndvqgzpf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kpptsjcq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jorjmtox.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2uxdfdjnq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2emziujep.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2kxzybisa.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2iazfuezt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2etogqiww.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvtvhwfq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tvzpkcvw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lcimjawz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qvofbrog.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2uhctjvcq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lxczjkxa.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gmtbhnbm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2tzltksru.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2kfgbcpkw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dyrfyitj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2abzkcinb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fwddgwms.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kllohclo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2skiyxdxw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vzqavnoq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sifrkvjd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2zgbaungl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2nipdvqzt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2tqnbrcvz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jixgmowm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lejiuaou.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2avpjzgkv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lwyplzev.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2znerumji.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qpnovecz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yxnwjpui.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ckmaxzem.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttnnvood.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2effutqwk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2datsvola.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zxjwtyzr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2psmjnsja.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ghosgszj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ouybfhrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxfngbnn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wcjhjjga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fahkflpe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ldrowphp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jlbehyzw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gashbmzo.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hydbsvdw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruxmkkxn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qkkxxzij.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2fgddeelz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2viaoebav.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmdsqrwp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kyqeggbe.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rnfighpv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2nzdjhewx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwhvzpow.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxozwpmb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2znybdryq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rizkrkys.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2dsntprrx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yuridlsm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jasouzjp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2oquyvfvr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2uggoeufs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2amdvjcvs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuzvjkja.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxygjkni.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mjltjpri.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2brurtrwd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2balztkjj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2caqxoigv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2wotnaikv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zxiahxqs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlydmynj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2otrpwfei.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ugcnheos.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wkgbamff.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aekozkzu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmcyagy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lndlrrhn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xntxfbdu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kqyhplys.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jnejvztw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2moyppbjp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2uqhkcaii.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cwqlbtct.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qsguphmq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2pyhtwrqf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xpkwdkhu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pnhgqipi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2toijqwac.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nqzcaine.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ijwwemno.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xampmxtv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2znvxakun.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xffanwih.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kxvskepg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2orillgyy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mbgdrtlq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vahtrofz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2aklanxhd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hmcbnbbn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bfxughyw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ifmxjrlt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2myoiohwz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2iktsmubs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dnqgzvkm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gpujksio.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wepdoctx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyeawatw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebhbnezy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pbvxtxbu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2aubsgiez.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2trfotoeg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgcfgifr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nskdlclx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2njehymev.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdgrsgao.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ihpxqafw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dvskynmf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sejjdnaz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kgsiowwt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2prhnxybu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cklxaefc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2eszntgcw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2dkajemip.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2rrlkopob.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lewylehm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2onkjwtap.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qshdcyxg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2prsywljk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2khqctfph.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qompayrp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2iwznkjnp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mmflpsti.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2axbrycum.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xjbjatct.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ggepdewh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2qcknyhun.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2gmhycpie.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mddjcukz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ucjcnayy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2avogfbdu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zvcnbgej.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2igrhoapz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vlvprojn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fyimczrc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wuuvvdjc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2erqlnjkm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2yrlsytis.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yhebcphm.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ybhsocfg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jxjvkpiw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xottyfzg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2sfogzaek.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsyisyqe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dubfxagz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2fpeybhrn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wpayrkcd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bwkqzogw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2itkwfpzh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kllpscwi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cbczwley.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ihxuwngb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xjzikgpn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2snsyrhde.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kxrqidfp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2smqhftpn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2oiboduil.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2nuttutlm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2efvdfism.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rtvvctva.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyyxqbvw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2yqneoxuh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qabmvzbj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gjmiisnb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zpuxchmk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nizdfpid.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qjoyhowh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2bvajrrjc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xwuezhuu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nmbvprdb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ecfvxzex.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2emgmmodt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2upidbotr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lgwwuggl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2adzvqkcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzysagsh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fuaenqaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osivtinj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wsgnacax.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2pxaycgoh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kcayekhs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lyddgubh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2imipuvyd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nwzerlra.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2nlmtsgfc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dvxzheaf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xuojusrm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2lxshlvnu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2edrdiznf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2thymenpl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hgpwnqic.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ytitfdyh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ldajdntx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dzafduss.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zvezorba.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2omksozee.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ckvohrza.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ajnrsuvx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2bcbqitju.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2vibkxtpn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2drwwmkqu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dvarhyza.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2doukmpni.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ddodojwp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jwmwjvrm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ppibfxxo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xsrupxuf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fkxvwozt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mctdlecl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2huoqscbn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bitlbbtr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ulnjlrpr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2czxjdufz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vjxiegic.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zkkaombu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zrdlxqiq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2suwdgrzf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lmlbuvkb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2evuvkekm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pkfsvxep.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ciqvkyhi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2oesamazs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jmrpzhib.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kgqdvevj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dxdimbvb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2brptqdyn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2riarovzu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mqvgnbra.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2igpvlaup.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mukudvtz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pdyzmsrj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2oyppagpw.html


<!-- 参考信息 -->