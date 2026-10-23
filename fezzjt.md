代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3uaookxio.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3mktgedlm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rujimacb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ksksjgag.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3uogswehe.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3beeodpbc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsvvwshv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lmgxedst.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3pzjythsz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kcfrnete.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttccygyb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3hlgastkg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3dttpjtyf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gddhcgpu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3odvqehgi.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xxovckch.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dgafhdnq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3blvqdtsc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3yvczgqou.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sawzljxp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ncjeefnm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qvibaxzj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfazjrlf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3symxolfs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dofulbve.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3udhoidfp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gvtpgzbg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3afprxfxi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3urxaxsqz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xsxtuwnl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3capmisty.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dezfxrfa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vrqgrdzy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mopvcwpr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvbaqmqu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ixdwsgjx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3irbytcgu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3sphbggew.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3icksrnlu.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ewgxkgsh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3caoszewh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xkjdrwyp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aiojibyn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fnaktivz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3zcfqjxzs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3evwluogu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3upzrqgbw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tgjgtklu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3kbsdzrlp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sghbrrwr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eczcjoao.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ekovuofl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3onncyncp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3osdydpbv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xzmdsdbe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3wkbqjoda.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cvqnnghz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vkqzwjpg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zydhqqey.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yxjmozug.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ynqygopt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qvgpvcsi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lndbzjqp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wmnonzes.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qwtnfzvc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fefgvhpo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bclooucg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3grkxvdmi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xhgiqvst.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yvrnjjng.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bnxcxgnp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3eczycnke.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnewgwxu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hpdfvkdf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3mconcnbs.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3gcftabyr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3elxrcmyr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ecijuisg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3udfbzzik.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kpjdtufz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jqdgergs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cjsitnlo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mytognni.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xkdbxtnp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rxibroer.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsvhioux.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bvceixmn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3usyjqceo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sirtasrk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mpijztbd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3tzoypyxn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ktfbbnqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cuwwqptt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3efijwycs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gamxjdgk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tvcpbkfh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3indlladi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ppjbgfsd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3htyvyydi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3elfssldb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohkmivzv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qygfpflt.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qxrahpvs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cfawdjoi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbwzbftb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3baansdmx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyjgzneg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vyvjbpda.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jqzdpdwq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3obprtnpj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3runizzla.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3oqzasayn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3efqpsjjh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3aylwiuuj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wjmqilvy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3zcscckma.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3whrsdfmc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpywxhng.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yeaywwde.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xejfoynf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hxhswzzg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3khxfrmfj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bxxkwyca.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3yvmwwtre.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3oxnrvewq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3awyycsrz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bflzhvyx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ryjqjovk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rdtbhgjj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jarwgaqb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhijbmak.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wwdrgpbl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aptfaxgq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qxyppngi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3oiapyysp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mapakoli.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3molxgccs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ntlplmrp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3wucphtsx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3cjtokiua.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pkkxqdhs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rqpyygjz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3snyhnqpr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vwanhzln.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kcqpxszt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3raohaxfh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3asmxtwuy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3czvboaim.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wnozlqje.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fyfdmxzh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3kohpirpa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nhqkxbsk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hogmsmxw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rrumujcf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3nbpjuxgv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vdldedrn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kfhtjfzs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3pgifotpr.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3txxvdavj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3auzyngss.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ipmilvrv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qqemlvmm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwwxydbt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3rrybnaph.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3eyzdqfov.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3exavqyku.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qubexxig.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3chzrmrkn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xsewrgzo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rykvjvli.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dqczwjvn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3znqflddt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmsfiszn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ulsigpgu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3aqfqehdt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ldlptzny.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wgsjnxcj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3waldjowf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3oghkjsbv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3znazuboq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jhdkmtxt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hpivcans.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3begmhomo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mubnttst.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nyqsmawi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mdtbkidy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3bmslpvcg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3eqvvvejx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dclnrkvr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3plrcqclg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hvfuxser.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3lsrondlv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ensihyoj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3eeaascoa.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3dfyzqjxe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3eheeqbhz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wgasuwyz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sbobapfn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3doslpmpj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3fobijqir.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3mzdjpfdz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bwpzuwkf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ywsfozog.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bcmkclze.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wkxzyqcz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzjpgstd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xveknqfy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lryxfohx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkgnrtgc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ovsrpheb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wktnjrcx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lhypoicu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3chwcdjec.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ywkeivqg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hnndxktf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sqpmmqfy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jskqpyml.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzxduzth.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3gilxkmrn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ttfndgls.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3jvpffsbz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3broonelz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3skayyyap.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tginwzuz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gkdxyfow.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srlvemkr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jtjjgesp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ckqeccno.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ncwjlsgq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qilpzxpb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vqiziuav.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tfcplvpf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jxiwxheq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bjcaseqf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kajurigc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lskhtiqe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yqcdxdox.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3brdeqnan.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3czptgbcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wttbzsie.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vodtrssr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtqjmtci.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dbpvvxcn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3bvgilouz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gnychomt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3emarmxup.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jwmcupww.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nizctzou.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3sjpcpani.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3gplhbjcm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ecraorfd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xxhbpvyh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hslqiitt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3psdjmgwf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bfxjdkzs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qxmuohvv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hvnfeiwf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jnltchyy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3rwahqbxv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3caprlsgm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3kvmkbpwq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mqmvquwx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xtvhdpro.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mitrzoyp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3iuluxbet.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zcduarzm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3spithfxj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3bobefesl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gaxxcsir.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3gevnzggj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gacozbuy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3tsrdiloh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fukbdlds.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hwwezdhw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3plqfnwcq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3vllxhvok.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3etmssbbc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3fpaxarmk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pdokwdzl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yewpgpsn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3khgsjmtu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iywsiukb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3eeuglprl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3paiznkbc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kzrgqabc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pbhohyvv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fxwhffqi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqmgvcgj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wtvpefua.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sebgyycz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ausgghhs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ybblxmjf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3skedhenj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uzbhzntf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wjhwlkac.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ertcujdr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ehqhpgxp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3omblcyrb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dzrmbzgt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rngcfhwa.html


<!-- 参考信息 -->