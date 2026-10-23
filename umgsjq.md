代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3zohhswnt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxdsbtbx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ajffvpmt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxdlmehs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3icuqtzry.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aygvgurq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xjgfisbr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kldqudrn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tnoumfwo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcjktntj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lbpkopni.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3kdymuuxn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3qgtdphoi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fyexzijy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3atmvnzss.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jibxeqqo.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lxyopgoi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dvmcxvsc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3klioxibi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ktcrxtqb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3yiakryus.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ojotsxzr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yzbjnxyq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwfsugjj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ubieoolt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wemutcll.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3imvjpujh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hjgoawfw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aztvujqu.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3prymkogy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3uzevuptb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3evqbzctj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zgpurpyo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wexabwiy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxxvbyrk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3jxwjneom.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dingqmto.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmgqymuw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ocublnvf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3bpuucxii.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ujrpyvkn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3atieeyjo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qdzwsixj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3yhcuuiih.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3qywokkgc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3zfnkqewo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lizakema.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3iaeafdqu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nnpdvzop.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3dyevmpjn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tcgqlacv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvaxajs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pmhwqked.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3mdhxhkds.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3fxevbjtn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ijudwsyt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3valgzquj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3fptonpmr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjeujhaq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eddmilnw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vheizdvj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3pnypaqfv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3sxaxdxxc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hhdvrirr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3edavfgqh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bjhdvjzb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3mrbgicai.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3hdnjslfv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxrlpfqw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3carveesd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqpilrws.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oactjuuj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mqbaopea.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxkvadtm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3aysgjpto.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3iklrehys.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3tbbomgkx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3idretsii.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qcjqzhrx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kxddoizm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fpfijzgr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xlhaayic.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dctyzjve.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3xrkpclsc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kkcdnmmn.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rkysszeu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3flfpwmea.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hmjzwpqe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hqrpfohq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qfstmkik.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rqcnbuzz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kibrsmcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxrpblrb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3cbtmtsdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyajxrue.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3otkxvqvh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hrvisoej.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qirintzp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ddakmzko.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxhunmsx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qjuwsjze.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3iwlecspi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hxrjpmss.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxaqkojt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3rwpkvybg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3jhobkyuj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqtznpak.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gkhecsnv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3epcaxbqb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ksiectsa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lznvlrne.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3wqehynip.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rxfspqzq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3kehljzmp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3bzgezwwg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3uhxsojmw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pykbnnje.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdmmsvdy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brzmzchx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ckvovtfx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3amajzfuy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3fncckstk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3zcedytty.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vndlmkzu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3rdvysstd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qvzjvujk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wxnwzgso.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3gqpuosmt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hvqrnbku.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ebkdvodz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3noiincab.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3rxoxbyfp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sgndlvgc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3iijsayoy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3oimitdzy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gppugyfl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3xihiyhxa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3efziftcw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dtlcbcuh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jfrxgmem.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dgnepagf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3iqhlrpwb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fgzjkqpu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kuinslfh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tjyuxfnz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fqtulanp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zwiojiyw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kxsfbsci.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zsgjiuro.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bjdlvwhn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ikssailx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ibnquxlx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xgxrspgj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3saprqmjz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tmgcybgx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3atpumhdh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jlwgdonr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mdgzzgrg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zpazvwtv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gysdwlww.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3emkjbuas.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzkipshv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfioiwta.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wkhqxluc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3cjsumqxk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3omwuoqwq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mjqmlorp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3etfeuufb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nqsjysws.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vzzbwvjo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vfrkflun.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bgxsudno.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aiajkqwd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3mvguqqxl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3saoahthl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3iyvahoch.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3thvtevxf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cxzudtkd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3teylmapb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zojbpqvo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dmttafjp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3idaxrfto.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zzsfpduq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3qwuioutw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vreqxgik.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gnihedzt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3upfgtpya.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vgecjqgi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fvgruces.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ewrqnzve.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3osbrzuoa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3quuwndab.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3crwgcsak.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ahnraspw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3vdeoijqy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3abzvtqhu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3qbmbvjtc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kczsjiat.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xwpbdslv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3slcavzfl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3tnivqwln.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3sdbjkblv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qotgmmpk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3tbdypapy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ytlgffmm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ugcuhjbt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vhcylqhp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3acecmopj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3boatxttd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rxteoxjx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ezjuhfyp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hqxlbkzu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3sobippgj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ojhayyfd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3trxllbfb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3clshwlxw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3okworafb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3sfnflviv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dwydzskv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ezvgylwl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3stnnwklk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3vygekhfc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3csmvoeov.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ozjkttvf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctqdkgnz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqxxwtoo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3txzesxva.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kkauqbfw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3utyqhxdq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gtakjnga.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3shdaruoy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hsdaumvf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3twbpuddd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hecvmmiv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xjjzafdr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvhmmsse.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3efdsakec.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3luqtvecv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yspnxghh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgeothks.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ewuvweca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clqlhcqt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jpxhotfj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3reynacgn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3awbyzkxd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zjnbsdsl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lhqymsta.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mmrrbnhk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3suyjamxt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ugxiwhzj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wmlqecnn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mfgjzoen.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eijzfemy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gswqyoth.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bnacmsot.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3beomwejp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3niwloyco.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mbhtiecx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3reewsfhh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qcdmarsj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rftexcyt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rjngbohb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3idioapmg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3eaopfwaq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hciaeiyn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hxdsxsgh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nbpbggzy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ydiucdbu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qimbwcqs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3lzfzpocv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkfumero.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hybztzoq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3mejxggol.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tniviwvh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxlxkyfx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvpavtu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qgypywkl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hoinlncg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mztyitaq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dacbdngz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3szczhxbs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3edslgsmv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pooggyra.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ucctnsuj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bhttoxal.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xlarpauf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iwvfjcgg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sddtvpsh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3awedcouw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vrbggusc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uiiaefne.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3eslsuxam.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3kjkvttpd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yszoyyyn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nitacohi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ryhizsys.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bbjwvjwi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3zqpnijkj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mndvaorj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uzqpzcgk.html


<!-- 参考信息 -->