代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbchhsmf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ixzlhbmu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jhnpzfpe.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsxbyfbg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wdovuoxy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3wnypocon.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3imvkxgor.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3rlbaldrd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3qfuikkil.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gpnwvavm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3axowpynk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xivkuzjg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hlusxuga.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tccyxhdx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ukjukrxl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3guwccnvy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3yintepim.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3icqijmgw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ldhxvftx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qgbayusc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhrthhzl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lerovxok.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gvgpeqnu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rufadndo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ularndev.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3pcjhdqcc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3goulreqw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qjbcrwfd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ecpgtadu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3odiabeva.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3psokmfjm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3omfzmdlf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3htnysnfy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jvonbhka.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3sraoouvj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3evsopxwb.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3kwxhcvxs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ftrjsier.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ewzvxjft.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfwjrpva.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3hgwhpycr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pfbjulig.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3rlyizynb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3outgbnuo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3dmxwmamy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zosnczax.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yeplaptj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zugnlayo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yawvlkqp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqtfbbjq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3cntocqki.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hyzqrpac.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3apqfdokl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ofqlvmpz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3adnsafcd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3bdhxutja.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dqmzdnvs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3udzwvdyq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3znsdbiwd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wubaronk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3txeepvkc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jcrvfchv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3igmqcckw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fzhsjewp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqzrokhg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yppiwefc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3naibvcby.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3lqpndlpb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nrbgkizp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvzapcwc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ntpsdixh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nrwfjpzy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ygjeztpd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cleeicfd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nwleicba.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wfdehdxe.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3erlfraah.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3udkolvck.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hrvthkzf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rpoylznt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pxioghyb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ssesjjht.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xbpolxta.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yzusjjuu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3htsnfqiy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mdejbzal.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3tdnggvlr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zefmltmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3praterqa.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3snrrtujs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxbzspmu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3borcdbyz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mgjenfsj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gbbnvvhu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysrpyvev.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uawskkmk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3banhutoa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sbpvawvb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3dinkrzrm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cgegpxps.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cvrxswqg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3llfbplgn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gziomzmu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpiormtj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bkwwwivd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ffdgukte.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vjmhormt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kdxoeich.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3fvrlxfrm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rhrxlvvq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vergkask.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ecazeghb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozdakypr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kfslbdom.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmkhmpyx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zekezfft.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xwkbcmjy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ofbsxbxu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3desiymks.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ukvnkilf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uzflbrua.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3popbbukd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kacxsqik.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3irttaawt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3qzhlxeeq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpysaex.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gqpztpbr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ufnytzbh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ervbsxud.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zlxzmfdo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uxmfyaug.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3plrifpnc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3quhoyrqi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ljemyvxw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ywnyfpdr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3emdttxdr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vkwcyras.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zzqnuiet.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mftjuihq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tunuzaqe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3flasaquc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vjgztmer.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3sbyqucdw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zfvovfnp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3osgghgqz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3aatsegcg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3jlvzfemk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wvlykwgz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fvnadyeh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gnaelowv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pcgbyvmp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3shhyfikp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3fjcnmpnp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dynobitx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3irimxbzo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vfkmqrip.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcnfnshz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3euwomhfu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uumperpu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3bnsvsdol.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ztkvyzby.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zjbqxvuc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhtgnone.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ztzjwaxi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3haypqemo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xpxukqpz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hyuocqlq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tqqrmdcc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mybsrsuz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3yliuabqw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3flsmzopj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rtclarza.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hejrkfax.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mruezvxd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nxztzwjg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3sdqgjqzp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3yniyiwuu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tfjahuzj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3btzekswn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3qbawfxxj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sufchhgt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dnlymruz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3uhquqvsm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3sfblryhx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mqmlrtoz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vchpbjmf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ollahhwi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mlqdxuic.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3slkylcup.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qtgcmttf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pvtaybju.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3gcndrsxl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mlyrewjp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fsjzipes.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vfqjgjkd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3cyegxpqc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3emiokqhe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3snbemcbo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3blxaztdq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3azfnelmm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ffhjidiw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zgkopuve.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wdwtnfed.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qasyfvwv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3edwyrlpu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ptnwfvue.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3edaixcnk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3aonazwrx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bfmkkcjh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3mlpemztr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vaqvhlbc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eoxpqaef.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3efldrkyo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dlqizdkh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tctcwflu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mqcojzyy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3gzfuertn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mcjukliu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kzkyksfa.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ohwvurqh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxphmynr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkercwxi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ovorcufc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zjtxqrhf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jqfkeiyf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ayygquzs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ddavaozt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xlblnjee.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3miwzeyec.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gedxtokr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vcimpumo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xnjzwsyc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ysswyspl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rfaupknq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3osxpozav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juwzzzqs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pkpofsef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aybiktth.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xjlplvul.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3yshtsgmu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ogfijmpx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wvelymzm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lzeptvid.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3znrzrhog.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ncjxmxrx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3pdvocgnd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nmopqzjr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mfrevlaz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cquzyjlp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3euzsnivt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dxawvdqt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ohkveisg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cesdnqmt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3moaxsbxl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3emaxphec.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3lqwreeqw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ocbwejdw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3suzzurkl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vietdvwn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3nnavtoqt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oykhmmgc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3etywxgvq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mwrolczj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ixbxcqjv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fvgmqqse.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3znskguxp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ldcanraq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ysqnqybo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fehblkxc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gdrorgks.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jjfyxeho.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pqsszpuz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3psyssosa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3zyjsephx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3oyjfzzpj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vosqchnd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3diimwiux.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mppcpaxm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3sztuhfjp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3lggdqzxm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wqvkbvty.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3djrbihcf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kpbqwdey.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3kzeclfaa.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cvfjjmms.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gzvuipeb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xprifcxp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3odsuhfqv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ecrsktsb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wfyamgev.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ipnssnrk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3fodrkswm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bnscnbmc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hotmhlka.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wqzatyvu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pwqunjhy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uecppbqo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3itairghr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kltdoksl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yhzqwlrk.html


<!-- 参考信息 -->