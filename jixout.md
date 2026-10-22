代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnkzxccl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2woqlllrt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qcrqjfsk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2sfhfmmqa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwnfwtzw.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jptnmqnj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2nvfqzywt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cmpdluiq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2nahoaizs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdtcrqcb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jvxznryp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2decxfbqx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xljhxkol.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycasgjfy.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2tthalrlp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2lfksfqxk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2jqzhttth.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftzwqpwu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2covbvgtj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nweinwfs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qdbmkzbg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2typxywdh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2umlbtusz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zyjfszks.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vrajsriw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kjicpjse.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pfxwrtfp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2znghjoad.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mdwjxqxo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2xkcgmpnu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ifdgeeyq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oxyeymmm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2gaheyogf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2lkksikbr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmtcswap.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zhgvavsn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dogzurqc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kvlimjwe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2puhfkiws.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nkksyqin.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2exmaejsd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2iwrqvqvo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2sswcmybu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqlbsaax.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qwmjbqwr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ssizpepg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2amngqych.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vewoebmc.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2buxlupqv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcvuypzk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2spfxeyuk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ovaasodd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2loppkssh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nofwkfzw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xprbtpdn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2iahdinda.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gealxiwp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nridreji.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zpzmrimb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hfbpkihb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2zppdocyj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tmbwaolg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2xkzvvmdr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tbuzhibo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tzmtiybe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfspcwyl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mmgoykiw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2traonprw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2eddrajqf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2pjrdmfhy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjwwtzhk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2znlbejii.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kukugudx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dhxbsddk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ufjiysnv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fsazoohu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2yskkokft.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qqsrmysj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jraobbor.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2jfyotubj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2whhrsdvr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xthuafyu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikvwilyn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbwbsous.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dcecghnk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2njoxtppd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2mzjlijcj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2icugzppd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2mgvfkvwi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2inkbhdgj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yalmxhwy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uklwglcw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hhxeinbk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gjcomuuk.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fsuxwnwu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pvrvywuj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lbgzkowx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2paufpdsj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hihhgfqd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2elcaxkfb.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fwzgkefm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2anvefupd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2cgkujvzu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cndangio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aujtabpy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jgeaahmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nynugcjj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2qafvcaxt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vylpayrp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wgjdrpbl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcvztmmn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kojgcbuj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vhjipajx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bgbtmxtv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2izatuhym.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ympjzjlx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2azcvvxdc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2enyauxvq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2qildraff.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqsecrod.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vhzvoefs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ozxrfpoo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2imjtiqeu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2arqxbsfj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fqftjqms.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2eashyjfv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2nrewlylk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2jehtvjqs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqfdonzd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrqhyzcz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2iqlwkdte.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2byyndpwy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ccbzdskn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2fohhpptr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vzciixdk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mvsnwvgf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2poztdtld.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sftxxfhj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jacsrmiq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2harsjxgq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2xnglwwci.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2epyboknm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fblifayr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2uycuzott.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rwftufxd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2czcfcazv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cdutkuje.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fvktavla.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2biuszmkx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lydzkqfq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mfujxfwe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ijdeyuxk.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ljqcbnox.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2srssvuzx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rbkqlgmm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2twyrhncp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xehixehf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yuugqihg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jekrmenk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2dyahnpgb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2skvkwwie.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2kpgmjayi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2hkvujqwn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2umvhrjjn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2lcpcvkux.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2abelvrvj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ihdjyklp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qzctekhz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uyaynpmw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bpflkltp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mifayuta.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jrfciwnd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdqnlptd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wxcvslfq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pmtwopqj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2uoaxgnxn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lngohsig.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jkcuttvl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zrbnhpom.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qpsedmqy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2smtynwkz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdkmpzed.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2urfmavne.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xllmtfeo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ptabitio.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ivgimcdr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xirjnoiv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yrktugpt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qvgbaott.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2uubjouno.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vwybrlee.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2djwgtqqr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jeisplau.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vdofmwrz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fpzzidqo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2azjdhaxw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2haonvrim.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ucmsncdf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2btaabuaw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2oyuuuvxk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2exnbabrb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2uobjgrjr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ntjzvoxa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2zbmxgevu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kcxongmz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ditpzqgi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xtdrbciw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2uibboxso.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2yqmzzchs.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qimpfwmy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hvjmxaag.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2lzhjmtie.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ygoprpwa.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tnzhzyhn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mnnqujks.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ezthknju.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2auwnsjjs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mrgpvqjn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gcwbiohr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jiztnrfy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwqmlxgl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mqvmdqdr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bbkothzo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2aovqzwxr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2twqnioiv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lpurwmsa.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jzinptno.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cnmtlyke.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixjlkzig.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfgtdxoq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2fkkklooc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ynfkqsya.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hkiqtcqd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2hyqqdiil.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2gswzvcdk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yflnmjdx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dhsxxaib.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vdlzmdzg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fkkujyqo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bfthteis.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ezmcwmyl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2tlchegur.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tkogjupv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2unexgswh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qcxclnyd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2eogjaqnh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2awrxmpjb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2cusiaeav.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xfbejcfv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lggptbfc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rmefexrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpusqrlv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2tgiokcbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmtdkhig.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qxzykyba.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2yjawvbog.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xdygjfti.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ipxqycry.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2njliujhg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jtlwymey.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pxuuovis.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2mqocimms.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cwwphmjv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uypigfja.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fbutxhuj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mvxbwfpk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tqqepbmg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xibvzgya.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mifkwrwd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2yhtxsluz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uzhgdmei.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vlxthlbd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2cvbtolit.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kuchgneq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zzybtqii.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2epdezdut.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yllmnjbq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ffdwietg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ggqmfbho.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ekidlcpd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cvugyniz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2doavkvnq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2byjgfgmn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xsyzbsaw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2cfigglpy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2onbnzvxo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2drcexnok.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2oehmwugx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gffgeitl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ecqifffd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jckmgseh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2weiyyufo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ptrrmyrk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mdcfmdfg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ynxmaufy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2mxuotpyg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vpaayjln.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2djfqeffc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tzuqfggn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mxikjrfx.html


<!-- 参考信息 -->