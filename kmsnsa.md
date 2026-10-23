代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xribmglx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ncedtbtd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3smikcbun.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ilgwfxto.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3nnzkgtub.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zkdfjstc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ixluloyu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mogfdzbv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3pgkrejva.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ftcuwrmh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gpmikekt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3npoazxvb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xzmrdwmb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qogpqyae.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jxvauglw.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kvqzlsyu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jrkrfiwj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3myvhuqyk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3epdlahux.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3svzlqywf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3qgjklplo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3lkivecte.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjnvlhwi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qconyxcd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjmqnklw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kcjxibtu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jufeyebt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xjncnvrd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzmfxwyz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xqasgaeh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dulknzed.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3nmigkzaa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3otyiqgyl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rwzhdssm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3uwmxjrfk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3cpihtkaw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zhfuegmp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdtowlth.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gogubazd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3hihizufu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3itqxjenf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ctldkwlk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uxmynwrk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bmdccqvf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3iiviezve.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3abvfepeb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ztvmxwpa.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xztvxses.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3elyghxkh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3sylyybzc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hdpftgux.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yypepjnv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zmtqsjss.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3serliquo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jdatbddz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tlfvhkao.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3wkqdlnes.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3svecbatv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zejcanuo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmebqwie.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3koiogzdx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3copmhvog.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3elfwikqv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3buynxkqs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3uslnhsca.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3bsowwzyq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dptfgsum.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nuqpafjf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3glnqayjd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqbiqytm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3weklwrds.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ezoxjrvh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxvhcnhc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nfhrioow.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gbulxmbr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vydnqfka.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jpzmdyqk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fspkwpch.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aqlzruth.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oiwiqmjo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zwviozje.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ckaptvyj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3raqczrmk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3veqmzzgo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tdjreepy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqkjreun.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wxjopfih.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nkbfszbd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tmrtmota.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3romlrnnk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ftvumpsm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3limwquhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgafboqb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uprlwhtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzzbgowq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jfzscjkr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zkwbplou.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zrdddlim.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uxuuqvwj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3njpikewb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ypensopj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3krhljfmk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3vcybghxt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3omnvrqqd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jfqjjcpx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3jqvtwmhc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnljscug.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3muzfoeba.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyevwqcs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kocaloxg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3knbycgpo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yivndayr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3rxhnapjd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3bdjhpauo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3vrhfymoj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3bikmhgmu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ephiiuwi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttswrdib.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3muolwqkm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3matkglrj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kcaoigbu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rfcgdwjs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3sxsssyso.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tchumqwg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bzejxqbm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3efnbohbt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3dnunyoau.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3oywkiuic.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3oiejoglx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pjlixlod.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rwsyslam.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3gihqhnhy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xtqxlsei.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xiyorfbc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jngssofu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bblfqcdv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ckjtgdjp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3unnwytvl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rgarunmz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3uspjrsbe.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mhtyfrad.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dtygxeff.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ldumpzvl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sziiprml.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3egkqsjeg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xkfkaatv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zwnmyinh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dwmpcdzm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3akfusmio.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3izdxpfjf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3feavpjiv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kvbgxzxt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dizoopsf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3weczisfq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jzrmbkam.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3mtozluff.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rpjtxigt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kgufudcs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3amjwfjfu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3htjehvfi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlmglmuh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qnkugque.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbkghccs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ntmateyu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zwayhsjx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3lksbmrfs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fuaoneli.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mqlnmpbv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xrnfbjjk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhxlcbdh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ycwmgixy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3foprpuus.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3krtjamnd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kvkwfbkl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuzifhoc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jixnkmdd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kviyopol.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3fgafykfw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3igpprlqz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3fmtvfdmu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3flcjmnok.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eaphhfcp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iogdmgbv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kmifoyrg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hmzilwqq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3njeznifc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rbxifrus.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kdifmppa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vipcsila.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3oscxjlfd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fidqqole.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3onirkcme.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3yotzkmra.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ghuybwow.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qghwnedd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3plvegohc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3pzceqzag.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pqnwxqse.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3npsonwrw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3yszersqw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mvoutpkz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xlnnjibx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qqshszth.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mbhsdgkq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3nhitkgld.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3usnfzlxl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xcozmqye.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nvnvijkz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nxkjghoc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fahunwve.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wzlcpbbq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3bheohjph.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3lzvcyawz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3flwxrmpz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gauuwzaa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3delrgkjg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxjtdqrc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mpkadvgq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vnoxfvtp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qsyyyajz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xdpjsjlh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3adrkelds.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dscxiuwy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3meghtesh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3acmcugbp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3spncjnsy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qjjguyqj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zqhncmtp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bwxfibob.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fkjhybnr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rjzarzxq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3gnppzqnm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3drrpaamt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jkhzlrxu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3kkkjidxe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3segqszjb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tznqzcnm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gxznnfrf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upuvbwnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwxbfffo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qbxjzhsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnypeqkw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gicwfpei.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ywhptkxw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3djgnvsti.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kkzjnjsj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3uughpxgl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3upkiltvm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3esihjlpr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3doghmtah.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3oxjrdowo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wmkjkkwi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3aksugfgw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lrkknkgo.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zytvnaou.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xnapoezs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fyqnwhtu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cuvlbdvb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3oniotpgc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xbpeoxhm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3otggghir.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yylvjqxm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mzqwwazx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vkcyxlnu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lykbiqil.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3llkvdnjv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ilecicnd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3sromvucg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3abvuzobu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zlonynuu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3invaixrx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3trtsmnke.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bblcqxao.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dfsrdmar.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lqycuwnt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3khyxjanc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ofxhufud.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3bujawioh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lwuqbybi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xacgjloe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3amyqweuk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fywwzchl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wnbmjmrd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iotdpwmt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xojjjelg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3inhrwkng.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ojekypsk.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3llkkduwz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pksoiucw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vtwzguhl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cksxahmd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3icihshjh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ybxnlgmd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3abutsmxe.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zmpuqahq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dlgdzait.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nahlzcih.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3daalnryr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ynljcpsu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3swxtishf.html


<!-- 参考信息 -->