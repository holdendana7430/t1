代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3fysviloa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ilmxztst.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3nsszvapt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jkmxwjxk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztrypwuo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hoxehhej.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlaitadm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3nufhmhxw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3wnjqwemb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zdzcnggv.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3utfjeive.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ajdqsyth.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3pgmdzgfz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wdufxzqo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bqtkvfpi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvnlgqcc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gkwexuzb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3odzimncw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rqftixgl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3cbbqzujc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zrsblxev.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jgbqrnbq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rewiffme.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3otgvhrue.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qwycpxmg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3csnybvru.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3vehafuhy.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kcmbnbdu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3txlgqouq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3uuvqxjfi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3bhiuoqkb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylfczozn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wdarztwt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vvpubitl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ttomytun.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3zksddalf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3sbzlwzcj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ctcekxah.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ltaahgwo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ylboinia.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3iumazefv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3renrnkub.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynhuoybp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lcntxsyy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3luajtioe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3iadpdkjk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mxmhfonv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3eombvknh.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ytlsnuab.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fndsigrs.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fiahfjug.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3jystoplj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mxnkhffm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xfqtxjkz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vjsfvlwr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jnmnkjiw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3asxrtwak.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3iwhfcpyz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dqwywguk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qhfrbuyc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jlnkchup.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cbpwuzbt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3sklevxxw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3bzchrxhl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nzcxszza.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3janwjhao.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fvwrwhwz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zlzblhia.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3adwnrrxq.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ijflyryh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3umdpflie.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3nwnixnvt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3czsvtbue.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gcfnntzl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3tqxsbxah.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xuruziro.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3clkdkxwo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlhvhsdn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbgcrbrv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pjyvakhv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3atnumeoa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3afzgqwnm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gcptyizk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kyqiiasx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xoevoysh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rarxtcqx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hgcoohsu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bhklriey.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3omoedlfi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3orpyrhxp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3knjzbsww.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kfzmlviv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hhskuqth.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3luxwkdvm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3slhmcylp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zekmuowy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hnyiaxef.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tzlwvtdd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3cgmwmqta.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hkikjzkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgogxhru.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qhaccndj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvydgall.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cytglian.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jxxgkmzh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kunqwxys.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuhmbwri.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smpqkvii.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3scfnjniq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mamfaxjx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3exsfnncc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnifdfyl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3iztlnjcw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3iakzuyeg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dhfcggje.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhxuggua.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyypdcwp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kxggndws.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ounyxpih.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xssysmqj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hozfruem.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nyweldwb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dradsrjo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3iqypunhi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lyzsmwhu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nzexbfmv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bcrvppmz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3iyuhkutj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ufsgwuea.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3uoxmmxir.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3zjexkmwt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3axfqxpec.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3imiaifal.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtkvvhjb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3uagtlsxo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rpmcrjmr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3uwttjwlj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vwafhrix.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eridmifh.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vicldfus.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ddrvyelk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hkpekggi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3srctgnap.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hsburdru.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3xwwdjgkf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wxtylwfz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mrifbkpp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gpisfdqc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mnlenbrq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gzeqguzl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xjwhfiof.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kvflbmkh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uryihyqy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zqqkrrzf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jmnvixsm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mrtrljcq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qvgrraop.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3czzckfqd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3cfgexhen.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hcspsvwc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qbyzcjoa.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3bbuwrvvi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hmsdfodz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3patflvft.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ucldheyo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ysgkggnv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3unjxrqcz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3trkoijyy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hwkkhqyc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lejgzcpp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmersthv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3gfmghhia.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wttvljav.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3hskpciod.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jlfufgeq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3qinsscxq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwspdkro.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gvpfxrce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fiioffdi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ebbkzwzn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fnotmewh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mvalnlad.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sobpdovm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cfqlocur.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3pcuqvkjk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ffmqflua.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3uqrwsggk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3sivjwuua.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fznppuae.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mqjkkoxw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vxqfqkvk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3pdrqrzko.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kwdtotfz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xoxpmfpi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rhdsmmlp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pxmoaomi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mhealxhx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3fdgucaiv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3izlfknmn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wlmckafn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3shceelcf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3oyclbxzv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ovlbgdfl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hzpcaars.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3eexwjlnq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jaeyuabo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zsloqnpn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3eocxweze.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3dmcvrzbt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rzaeysut.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dkrcbzxu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3liwnvwuj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3fivtfjcv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3snffuaht.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uklxifdu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhnvkphp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnoqtkva.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pmankjkk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tkjpnbru.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fyutfjxr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3omuulqxr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qeagmmyl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dugdmgjo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yviygspl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hbadjtgz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3symdbhqm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nqsxdpyf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3whnqeswb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yxuxvqtn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qliloecy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3uwxuijmb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3nwwujkfp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3utbaolnk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zufptsgm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3njrdgdsc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ntukyvhg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3mlaysulh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hqskvllu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gbtkxdrm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3frfbtikf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mevvhqwu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ptsqeosa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3pinzhiwb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ichmvmom.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ymfqoxlb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xqtgdohe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mquufhec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ietvbput.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vvhvrvwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vygibkkl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3opfejbrb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3vsozwogq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mdpwrsas.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pyftpzwp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ztdecuex.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3uxaaiwel.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3oraxnumv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tczdraln.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xuosygqt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zjvyjkup.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hzugqlpb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fmbfrsxu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ketfndam.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3joackqzs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gycoziys.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wlykhbax.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lbfujzzq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oiqrxfet.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3pjzgaktb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dpfklrmi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hijzrxcq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lwhwopky.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hwvtspwf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bylxovme.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mmfvwzky.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqlzeyh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lrjkvtey.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3mszkaisu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ycebvgnn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nhimipwy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3juakfrch.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yyyrazkh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yuzdnahq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ggplekad.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3nlxzsxuc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bospoyhg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gmclvqyx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xiasoode.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jvtclkht.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3doqrlwdm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3iqojnmpo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3koazckzb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fbekekvl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mclffmmr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3raqzworm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wycvxivt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qleqhurp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ljspnvkc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gfjrqmvb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bivdlkbq.html


<!-- 参考信息 -->