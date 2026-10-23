代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfntkxor.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mdfhdjqc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3oaiipdxj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3uhachpkm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3jkvuugzu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3pcskdefd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bxuttvla.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qsmnlell.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3piujldle.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rjxfdykd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uefwqnkt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3etfiwkwl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3vqcrkpuf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kmvwyttp.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cluhhqhu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vxuoohji.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3clbbhpaa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rqcpasuk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ynfzjgua.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3imaqcess.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nlxkxslt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qynywwze.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3nlsojsjn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tpalddos.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3aehferkc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mxquidkp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wodglwpx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qehttqjb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ypucirpa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cffwvbus.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ptnubvzk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ibvpnkla.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhccapex.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cwjlkqdz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hmyhkrwl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3kiliyekg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zgmgscqx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lgcdoffj.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cqvakoqb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vejgxlsk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vuzsoeou.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3zjkrvttp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pcfehjsp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fukvwrjl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mtpnkyht.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uqfepxbh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wyvbnhzl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hxsouebf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3sewcpxmr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3usymrqll.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3spfizaub.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jmocbsuf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3kyswkvzu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3xtxnnehc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wvcvbrci.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ctraimos.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fmjjtngr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnyghhoi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nghtsavv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3esipgqxc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3geupvfer.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3gegjsbzk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3uaxiqxrf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ojnnxdsi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwpsqiwr.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3tduubith.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3oecjebaw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3sevipozx.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3dpoflfbx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3yvwarquq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mdmsjtsp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dxwxobfk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hgwmfpyb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhlmyljh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pzmjvqjo.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbbmgye.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmnjijpj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kjwudjiu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yrsjgiax.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ptkvvfym.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3udurjjgu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rhrfpzen.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3poaykuld.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hiqckozh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmsgqkod.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aaecdnbl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3buobovvj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fyfyxflh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3fouxsump.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3slxnjrhy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ljlauimw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3grgfcciq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yuwhgafq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hjjrvvpz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3otkypvqw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ubqsyjtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utrnozva.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ciplwxha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gopohqtp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mjcqxzzp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3rszwgnpa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tztjhflq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qjmmlmhv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mveumqag.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqsneyis.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3acyupsun.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fcbtorpe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3umnosydq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wswqximw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uscbfiln.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xyabydbu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dtpamyyw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gtlefluq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rmbeiduh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3lrsntqie.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xqstwbbw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rtvtcqes.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3zyuemggc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3bpjxoqhd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3jlkbmhqd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwxfhqzf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzjiwfdw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3asdtfmhg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3xzykdobr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bcmiwyfx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3aojofnoa.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rfijpeji.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zugxrfmm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3aawxxgox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdnapkqx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rlhgawcx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3xvmntztq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pqukluvv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lailnsfb.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ydcajfyk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3chhovavs.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lzzirjns.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3dropzoty.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sbxhmzmi.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tnxiebcn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3hcykrxiy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3emnxtvez.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3slfszkeh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3estzaits.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3siujuzan.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3nwglvbvh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tclsoobb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mlgjpsqh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rmzhjdtt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3sgaecuja.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ypmgigis.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3pegshtqm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fawusjfh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vgswfrws.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3judsdqva.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pqryimrp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3tqihopmz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rewlcrcd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3sywbfhfg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yzqhdsdq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3izsrduwc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wyacfesy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jjqxtedp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3aysbclqy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3immeahwu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tayrffyf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwchwvzi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3urwcawhm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kinidxsd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3psykjxdc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vltgcfog.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3dzedrqjo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqcechn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bpgjcebh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zvzcvcay.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jbfwkhie.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wpkapecn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3txensngg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xqrvxnez.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cccjfhjm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jrdjchvk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hcooppbo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kcofjftx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lwdvnyll.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3dfujbhfo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tozlbwup.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kouzrldv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3eevgmlnl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3byxeipwc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3qietjxqj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3mmgyszei.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wanoabtk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hzbhaciq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ukwmcodg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3cxzyzngx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3egbeiwro.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ghdmmofv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vmrxnafv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ubdlngrt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3vahavqmu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3goyjbyiz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ovdlyjuj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3femxxtmw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vyvfafau.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3nmpflwxz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dguahfin.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wfejwxmc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qqyybvyk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zbecujvo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xizsrmor.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3niadzkxl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zzpreuru.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifdvtxid.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3gzwbilep.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wqolunhu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ylizfxms.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3yuhymikn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3mppqyexo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dnpklrxt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qkhtylzd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qebpnysx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dzilyfbb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qhgineki.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rkryjryr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ioticnyy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mjiiaqms.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3gfipafbo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3dagqufof.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tolnnxhw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enwiussi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wvebangd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oldavtok.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nhpnqgin.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3afsrcpzn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3daynrvqa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3swmhybsu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ixisrpkh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3skbevdfr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kooqarkn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wfrqpgqp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zzstbhii.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3robdiwls.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3myaxgheu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivzoibbl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3atwrzzdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdgnudxf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zqxayyel.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3oupsanpz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3wfaziato.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tyhvsiku.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vycfgmct.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ybwjllod.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zgtzopin.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jrsyicnk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qeinnnhv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lgazlvlh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3galqbidl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wcawbupx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mpmqtkbr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3subrfgde.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3jovkhtxq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zohrovsl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zpfpyemt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fathxott.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jqcfjvno.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gnelxarr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3pitioyrd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lezpsfdc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kjvjjxdc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jrfflbjp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ognbvzku.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hxurngfv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xuixbghq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kcvojklu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3issjvcyo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mhpjythn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3sovqzreh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bipwksyu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hdwxlqgy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rvkzhthm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vvnoepim.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3oifsfdqo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ycpqrfug.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dpsiezgo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hmiavbsq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nzirwqff.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3lwupsnwy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rhrjlbiu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3asawrqyp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jcpiybow.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tmkmuvsz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vytegxmt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zuqcmxwa.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ocnquddv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ivnjzckj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ftjxdjeh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dgykfarq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3twqhesps.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uhzqbjdd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3otxrguyf.html


<!-- 参考信息 -->