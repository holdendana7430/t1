代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeezmxpq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwlnnxau.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgyzuhsp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3afghylly.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tyzmlbct.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gsoigvpk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fmrwvqos.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bniyfpgl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3vrnuntdn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ochgdhwu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fxdfeuwj.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dnfwfgct.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qzppnuki.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tktwjbnk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zqtkmwav.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kegogipc.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3taehqfqz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3frqngrel.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgmdhqfg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yflerqdm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3njsgbtnt.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jvyvrtcg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3msvushgs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3rvnhbpid.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zppojwcy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jccaovgh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hpsrfhrd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hrpwzpbk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mvumvtxd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3gijqnxah.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kwljsopf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vxgjtjbi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pclemrxt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oyhlusmx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ayxrnuoz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xduujmze.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ovswbheh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ruyynlqh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3eenvwidp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3muvkvlat.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3bsakntqa.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3guuhrvag.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3zgfkddoz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbxelqii.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gzrcqsgk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ztugdoob.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ghxqnczl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iwgtwrwm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ldnusjbc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fkuxtiuy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3nbgwplqr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3mhhxkphg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ubnpxlcm.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tjrktkxf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dzslctic.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3snazpycy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3drxbhjdh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3aftfumwf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ieynfdtd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3xyxrgyxt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xvdwsovx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3jhugernw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3plzveuhp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nkontrvw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uncfrieh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dpbwycnb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3giqgdcmh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mpsolagy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtvwnoxl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pyrpsyyv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3mlvhocnc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pstjmtzc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kdexuygd.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tlftgnwi.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hwibryob.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3butimwco.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ddwyossj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mltzcwzv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zoiwamnr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3sebyysfc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3kggphrhn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpkarttj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3buxwqvxo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hiislphq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fllwaqvx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3whexwmbe.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ysuovfdg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qwsdhybm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgqonpbc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ztywmyjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyowkgit.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ceelhdec.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ootavxvm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzgdxunh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mtlvojyp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovungmdp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sfkbospd.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3srampszw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3asiuhypj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eeeaatky.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3skmmvefu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xpywwxlh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3uqtjcpzo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3unysqxzx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jszojhrx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3webmfguz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rklibbdt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vxzhtjey.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3wjqonxnv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ghfwxznd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3beijmhhi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3oycdtmlk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fosvkhgx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3avhtmbav.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmxxwpil.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3dllwvbhr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hnletqlk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3sygcdwwz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dkqgnyeq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3fnujuyia.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kysmhaap.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ioexqwov.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kwacydge.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3optzoavz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mlhonogh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qmxuokve.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jqhzjmrt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qpyjsrrx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3udrnprav.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wpfojyjx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3brrgipio.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bruopqfo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3hqehpgra.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3epskcdon.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3eonkglyr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gusxvkmh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bsvtjdvf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3xcatpuvz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3qefnbtuq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hitgjaoo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hobseglv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rrnhvwuj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uprttzxu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3fkqxoenn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wzgiwfed.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rexayjov.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tnuqggak.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uaphwphx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ithlgnwq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qzvbtcaf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3aeblvegm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3icekpqjp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dconzsgt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ahwbkezq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zaqkykfh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3sggkuoat.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ljockqmg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzytdyvr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qtehnupz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ozyclckv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3yzyhzapc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3waylyaiz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3digdabyt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3diehhbmu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cogvfqwj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3drhngjjf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uohklcdr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3txjwibts.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3khhvnhfc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3jorauuwr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwgupnnm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3eecmhwbx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hhsaqwvp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tpyughbb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3atiqgjsj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oqtkwtzn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ufqmqqlo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dvufmobl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3isrzeuje.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3swnlmufw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cysbvrvc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jzwcqvkm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zyoxogcn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3yvdaipxz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3sepnrxxw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vmzpzavx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qmvbdwzq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3nriqjqrw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rajqtaab.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bxwformg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pdhufhxh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3faevivsx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3howhzseu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gitoepxp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iodqvvty.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3llfayaiw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zxsalajc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3novajpjp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kgljdauw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dhzxusfe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3padysmdh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3trzzuhjb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bnqhbhac.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzcaicrq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvaetiyo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kaczyrdg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uzcotivs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3uejegfve.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3nniesysu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wdvvojaf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ahkxcste.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ipzqynef.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqladyxf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3acprgsmn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3azgbrptq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qqrltgim.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gougibnf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gjvsieok.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kcnljctg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mvhtjarx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjnrkzxv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3coztlmhx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vfbknvsa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3voqslniv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3tieqjkut.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cochxkmq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qvftuwuj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nyhxcaxn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3onelvwxv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eoljcafb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3sijjmowl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbtzowwe.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3gxfmqpfb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3boekyhji.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3keaiatuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thjmhkmo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3tesrxupp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlaswobk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wippcvwr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3juyhsomo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jqjlaegn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nafglgdd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3zmirxxla.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3tulkxfai.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ukozjzxr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wzlqtrls.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ffnhmdun.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oisjfmsa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3kksktuin.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3outmknqt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nsmapocu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3owrnjjdx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zyhhubpu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wynkgbca.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mnalkfyr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3sfhcshwx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dfyrdcmb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pwfyoyco.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qyfarsle.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gfudoijx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zvyjkbzj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rozxkzyo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3kvmpxyvw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3loydczqx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3esydwstj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dkidjtvo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nidombcf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3muftfmec.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rwqxvtal.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dmdodwty.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uxibiyip.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3mxyqbghd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3waqrtbxu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3apnzaugs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ntenwkbo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mebchoew.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rjqzfekq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rewcclzx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ijgyulag.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3idaavccv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lzagtxhh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rmgaever.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kmonlhvp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wqdezogk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qlklcvar.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwwlohcv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qqeojhnf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wysplajw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vheowdgh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kgqeraap.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wxlqmcpp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wxdazfgu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3sttjpgry.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lxvynraq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3peliuota.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kxpsakpc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3filraver.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xjplxvyq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wioebfis.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wsdvidsk.html


<!-- 参考信息 -->