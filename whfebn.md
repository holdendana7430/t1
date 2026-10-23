代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sawddofb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhcustcd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ygnmsqrq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hrkhytga.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ernyjbpe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gltithxd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3xtugcpbm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qzoedzmg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nckoxyrd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtbtsrzo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3lxbkvwaj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qcviqvez.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ocpwohhl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfoysrnz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3trcadvql.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3byyphzaj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3qgrbqsfx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhrcldrf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohouhbjs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bawzoppf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3tnyxbzmc.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3qswmntjd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qbmcjzid.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3oalgjxeh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3holsvnpb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3umbbhvod.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tisawpjw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kxstlhzu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3sjvdvxdg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nddxluor.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3gsfhuuud.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vjianjmq.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3uqffhzle.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nbybfhut.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mochwelu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3szsqxfms.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zoauffoi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kdndjgkp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nxqadvzc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3sjgvkmve.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lhnndyrc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3qtqjrtng.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3nvawwecr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mivpjiid.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sycsslmz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ctjxolwd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xbvzjgix.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3fhuqitcs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3idxyyrtn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyovfkba.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3lddnyugv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3oatqfine.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qscflghk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pyzhzeod.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3igzttddc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3duwprygp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3xxbudlvj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qxvwqoqd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3igtpphvh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3asmlcfeo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jufecauj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jgmqmxay.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bnfiintz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iewbhppu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nejmmvgr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3inpboanw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3muuokjkg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3gapdynjl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3htltohfi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3xguijybi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3caetwled.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3skejoics.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbfjyll.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xrvwvxne.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ccfwzmrk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qkfqfkie.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3nzfkdsbg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3gbmwgzow.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pnnqtcmi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zqlstmnw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3unhzmaew.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3crqkkviz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccdyaquk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3nlghgipo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wbeceyhh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mpzmprvi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3imclhpuo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pmwagpgn.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rrvnedtv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zkoczllz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iwmtrfym.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lbduzemu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xaqkvudl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oguugolt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jfsrmppg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ifupkkou.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bgzxpizw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3curvhqdn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fmmsnbiw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wtvustqs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tscbizqi.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xhzimktq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ubkwneee.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3keexaegi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhhwbbyz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xrythczm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhfukaya.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yqgtatix.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3sdihxxpe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3umbitnmw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yyiegfad.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3faaxfgxo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eisjwack.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mhdbprrm.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jqdnrctk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rhdsmetm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tpphugbz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3keanxsca.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ftmvmxlj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xiwvxjbx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vcmlgvwp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3salwiotj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pypqbhdp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3lcbaablz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qzcgzhrp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tmqczwsg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hlrwqean.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wiosdnno.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnqocvaz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cyofkczj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rblltktp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3efyvwvkz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ffgkwqwa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3sttnbpbe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mqithoho.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3yhevvurk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3bofxsmsq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phxidgov.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rarjydcv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bqxpetos.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hflrhhwn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pewgfwea.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3penproao.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wcnadyte.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ceobqpsq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yrwkwkij.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yqadqfoq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rzrxctab.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zkzrquwy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jvgjtkmm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jnrrwlkr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3arclqnen.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nqzjjrma.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ukyhpasi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3eqecghgf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3usztovvm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qpowvnnz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vytjipwe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ibqsnpxz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ltczfvfa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3shesnqno.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hlyorvju.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3fulzrlre.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfjayvse.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3krtqhxax.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3mybgqgnm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3eowmqapt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3uknutgzb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bybbwcsh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rvhqkrea.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3soacdkwq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tghuptxp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmvmwavh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxuyfddz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yjsuktpd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3kkrqycke.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3psirxqmk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kgarrkye.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnrfizha.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fhgmwuyn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pkywevfs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbvdtwwf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bljzejyq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kfutumcn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jyipmjje.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3jxxnjfqj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3crajcygu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3eefjqkpm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ykpkizuq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kgbafffa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3cxlsjefc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3hrjdsgdy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3aleraobe.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3umbcxoqm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zjalcwna.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lqfbvzfe.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3brynlkzu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3cobwchcy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3hlbqmnep.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lezuiyrb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3wshqsrxr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3jsfowyxy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3svnxmgfb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3txarsahm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3owfndjdn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cflvcjas.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3aemdgdia.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mijfytmb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3qwtzobak.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xodysajf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pdabpqif.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3cchxftpz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hprrheuc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3yrkxohrf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ntzynsga.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fqlqswtg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iqdbfsua.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jmuhasmz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qkjzrsdm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zacelavx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ezrubtzo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ggjdotab.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qltfhbat.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ilprgqrv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wfmcpefm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3izuhjawr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nuydvklc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dscoaqok.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xassulmt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnbypvwi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3iberrbkh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3uqttxxwe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3sdzptmhd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gskgdgvk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hqevaigq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zguwlurk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yticmwdp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xdlljfnx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qlcxeshf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qwofoslf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ldkcafxi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zdlvhlvs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cgjndnwk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cqmpllca.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3toyejduy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ldnhqsmn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ylqajokh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rndjwesv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3vjwvlyhw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3bzkfdhgn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3lbvwcxhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejdkigsf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dzqqvdyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndrgufrc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sqrscmqz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xvyozbit.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mjjhvnxb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ouzdacdb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kditdcdi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wqfvxsvu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qnlwfwdm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vscqlnye.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wkflcnyf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ahimkohx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3oujwwzcx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3btmwjmud.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pznbkcxf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wjhmjzdj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nssquies.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hnuknyix.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3dmmqxmfs.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cbhdgwqy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wpxrxbsj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdweikt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rabtozwd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3cnxuhyfn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jehrwafi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wzwppbtp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ugcehmtz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3padfxdia.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tznpmtiv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3apgslrfo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dehwesju.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fuyiinyc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3hqwywysw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gjbrdjrq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qcwtauhz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gituydiz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3tcudttqt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3mpzhtnom.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3bjyeknlr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3flrixmxo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3azjvbdop.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ofctqwcv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3umnfkgvr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tudzrisp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ynedaxpy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vjjyvndx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dhqicziw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ocagdffs.html


<!-- 参考信息 -->