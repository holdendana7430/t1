代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3racafgvq.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3fjwgvqcm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3zcsklwlq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3msuyakfv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3scpxdlmo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsmdmmjf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwesxtmt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3eeiloyby.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3figenbbf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcmxhybl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lzgexziv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzlcwyuf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wnvwbkjt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ewpeqjia.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sekqxyky.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oagqnxqk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3lflcarph.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3avtpidzq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sempvhxt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3amtwtnyi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3xhgmolgt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nicwisan.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ktiktfed.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3blfcgpfs.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yekvowrx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3voatmaci.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3sfnbjlxd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rxzkkiwo.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3nxkjltoz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3whfuimqr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwjuabpk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nfhlskry.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cypmeouj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzafaegx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wxihawcq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qyovvxbs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ugtmnhyw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3zbztofsx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fslxynpe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmfvmxpt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eooynijw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cznxxuxy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgwbvpsn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wivkvfxv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mogtjqza.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3omhlvmvt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ycqbuljm.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3whdpzqsg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3djagvzte.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rbaactco.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3cqwuadpf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cdgopjdu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3llrtqhpw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3redumeyy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vciteyzh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tojrkkzx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bojxegcu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3jjnqcadb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kfesivsy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eixuybkn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oioooave.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3xowxzlzr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3lnlxeefx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3binykztc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3gaybbxks.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3mqzzvutc.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3liwbpbyn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ahikbnza.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bpsuwcgb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xpxzbfhp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vfpgxekl.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hspywojc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qsztnulr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3fzsvxtfy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3eggrpphs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ocszbqvw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ieshiutl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwbufkud.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bfkshvnj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rvezaqns.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dyerwbmf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mldffxdb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fataprnx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3aswjnpnl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3cxknkxpv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3heeuimpe.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yppyoyyi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3igwsktcj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rjgewlxj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3luwrohwt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vavwvsis.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3oqtcsddt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mtvsryvq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3osgnxhso.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ivstnahu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fxtdesgi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ivpagdnw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tqckdqnx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3aplanrct.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fdepxhhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zifmlymq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vvadsgzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwbpsvcv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dpedscjy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hvwdbesn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lontwokj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmzlclys.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvwrjyny.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmeryqpr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lowqwxql.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vwxqougf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ggsahaja.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qmqgwern.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cbrulrbm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3saokbfgd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqcfquva.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3snqbepvf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3tkcgpeha.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3taiykppe.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kadxshwx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xczmjfbr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3uaylchkl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gnmtexgx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3iirhajql.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3apkceunl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyrnbaxt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3boeldady.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3zqbccnjv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3shdkzqtz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3uhqyitxm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ycvfnfhr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3idvkpkbg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eccbidjb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twlgcngg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nwctxcdz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dgkqhrhz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fpimgens.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3igwfphkw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3adslczah.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3kuriowch.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lpcxhqhf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bjqdbclj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ebmgaqqm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xwdcbyfu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rxtofksa.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fhpufcxv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ovydifsn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ssdapvct.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3atorckvh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ahbecdue.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zxhgvzas.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ddcveubr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dbmaycos.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ocoxdqfn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tkalsijq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jyhtvsch.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yqzgebds.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xnzbmesm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3soriwcch.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fvympfuk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3juqvkyrb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fuvzalao.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3klzlawyl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3sklodbmi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jcadcrky.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hrnldqgz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3eutjhdjc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3fedenlpi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bguygduu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nxglytgk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3manihxpz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mgnrgbeg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wgjdcovd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwkmtxms.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnjzsgyo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rgwvtkuk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hilybmmr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cmzebony.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3agnbongk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tpxtryae.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3euovlrnr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3lmmywevn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3unhwnjov.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qypvbysm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ufkqejbd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hlaagdsf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3abtwltgr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vrdthima.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3aglklblt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uyncdqui.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yjhvfpqe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3nwqdztlq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bkjwnhan.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3riepyepi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ngrowhyn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ayppjkll.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cagxcvzz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vacmedrj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3mcauwdmy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rchdgnmi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3cdjpnzxe.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xicezrfs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3fvrmvugl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xgfsznmg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bjhqglmq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xzigkhpv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mkpsemjz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qhafsdzt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uhpznmuc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3nyrlxxtu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3hceghzej.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3npnzihvs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mqwcchyv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nlixgpep.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ikdwtznu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kztmbocq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eopmjlur.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3dedpyqru.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mkvwqbku.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bwmdpqbw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejidcihv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3carobuka.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gqeutiil.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nmkoctqe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxrkkpxh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vanhlber.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ymfqpahs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xbggwnnc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3weapbihr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pxaqremp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ndiciroj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3oehvvhrw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlawmttv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3najdocxz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yqvaejij.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zvfkipzb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zpdcqjgn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xqoaccfj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lucxevpu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3gttxfxrv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yxfefrmt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ayostivy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ygdazdqy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3dirffcsq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kwcplaha.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3onfpqkex.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xumkmvwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhlumouz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3wcpvehvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ialjygzd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ojggwfpk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jfcqzrxo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xpednfmg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pezdcalw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3glxkueiy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3frctaqfc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ufdyqepw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ruqydgey.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dmgqihoq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mitbvjsh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wvtzkvpc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3aenoftuk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ocyaaqlx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ltfbkvri.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rpxfabeh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ceffzuas.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3xwutgkks.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fwpdpowu.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yylxdqfg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3eqavpyql.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bbgwjmcn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qcmmpjto.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dyauwccb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qfeiyzth.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kvbntmlu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3yzsykhln.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cttbqiue.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zvltfzch.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3whuaibxz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fjgsvldt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rwpzhsph.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gpjspnwb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3dlxqjgyo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3smgfosqr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ioeptlwj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ejmgnoip.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3fkhtlbxe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3odmgxzms.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oznjnbga.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yslfeewf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ietiqobq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lqgpaqeb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3upmufqbl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3evvazycq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jlqnugbg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3uyuawqhw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbmleeah.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3remdwofj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ucjojsds.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3aujmzwis.html


<!-- 参考信息 -->