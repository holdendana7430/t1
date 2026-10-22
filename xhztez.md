代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2zkyogftk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdvhmziy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofxthcpl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2orloqecb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2xxnyhsoi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2stuwstsu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hqlbejel.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2gvjwhmvt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tppyikky.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ipsnnuie.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qbcyjjoo.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wrapuchj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uccwfeew.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hzltiubr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2kuzwuvae.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wbtkxtnd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2hzuvgxkt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2kavjsnvv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zptfmwnq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdsnbowe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2symircmj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2keinexaq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2stwougmd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rjmvaxcx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxregtcl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ixlordht.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2cklfajsh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nejwqmyw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2czmxmkws.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bbchtcog.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cxyqonig.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uyyaxagm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dhsrkngc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rhqrxinj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qnlftudk.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2sxqnkakg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zzeovhon.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2caexmqxx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nrpcrcfr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ftrxvitf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rdaiukbg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ivoczatj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ilojgilx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ualwrpbe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wleuxwyi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2colgxfup.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hgezsfoj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mruvlijt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rfrzkfjx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2oneguixs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2spyympkn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2ahladwno.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2gkvcocam.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xvznypnj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejwcfpdn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hufxhedn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zhxwrjtq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2wnecqmbs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2bdmaylic.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlfykae.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rvibudub.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fgcjfouj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ufeegdgf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hsybohfj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mrfdheys.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdpvxtik.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ujkekcvd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2oivpykvn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2paohbrst.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qlytnutw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zygearan.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zmtgjwbm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fjaytekm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2knlgfibq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dqsnhvlu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hzushltc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bqjtupxa.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tkdboxtc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ptjdprry.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lnkbnsqj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ywyuanoa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vfbpevnl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vzibflwj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rjfmmtnq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pnuppyfo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ezdnfrrf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2axuvohvk.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2podwsudz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atcqlzzm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mpbxnhwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkgvdbxf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2esuwgiyg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2eroffyar.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2xobdydcs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbahggha.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mdevtlda.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyoufwdk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eoncxfwe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2uccwfzzh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iviffxfh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kshlztcn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fgyafpip.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuhbuyyq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2luqiudsu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kigcpaeo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ojakgyde.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2slsvfmjr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2pgpgqbpq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2iahodoyj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2obfrqbgc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ixpzvbzu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jjflhrjs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ieoygbog.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jmpcdhca.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2qmednytg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ztejbook.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2uztcegpx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2unusywtu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2oqvhqvcl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dwmmaudf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jkwrfdlh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtzkksxc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vzgrurqy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2birnuyhz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hjcdfaks.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ulyumxoe.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ocafrzmk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nzokdiey.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ezbkbwgh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ifmhomwj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rmgbsgmy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uuajueac.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vhtpesyw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ojhyavcb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2efayizmk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2lifuccqv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mhudkzwe.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wxurlwvx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rjctchrk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uivfhnhv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rpzujjqj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rcgjyoju.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2svkqxfkj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hjfuduio.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ixjghdou.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lmpumdnc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hrtgegni.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pabnanoe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2cgrgwzhm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2aobmkzry.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tgopwxrj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2excyfrmh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2itttsmsi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2vpvspvbm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2htsxtkjw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vmrslneq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2clhflymx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ixywlgla.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ciwlojew.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2fmoldums.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmlkpuig.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kdmjbyzk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrqmuewi.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2jfpudwkl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2frntljzx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fnpvqqfu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2awbsrkyw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qzdipoxo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdjfcwpf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2fttzmzfr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhgsddvj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ympgrseb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2oynatite.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2kdnbuvao.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2igjpsfqc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zudlltim.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ohfmkdiw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zxkdiesb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qksgmbgt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zpbnqmyy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mvvjjgbk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qspdsdnd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xauaxgwk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2irkhuham.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jvzgqrex.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rgnbqnbe.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2fcrzmwug.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fjhlktzz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lbhkgejm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2yosnalrm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2knheewix.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2cslhnvnc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2igoqfpsi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lbrjeyoh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2byeosqfu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2osgfdpeh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xrlgoemq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2nkgpwpst.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2unvehrff.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dyvyrquf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pumluoos.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftyuhjkc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2oqbflhfm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ferjkwnx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymqgybnw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2yaujiqzm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qtbppbgk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kvsrpkao.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gvalzrgh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hsmmumxq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pyhboicv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2omyrylrc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tertzcxj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymbdajez.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wyziiwgp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hbhsoepc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hxvpctvl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2nvqijsse.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hqzwiaaq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zvjxhhns.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2hfwytrlc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2bejhtauu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lidjszmr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fsvkadri.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wyhgoozq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2sdxlroim.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2agyjfanf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fzbudxqe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bjtzfafm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2hufwvwxh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xikhqeny.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2duhycwld.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rphdniln.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fohkoefw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jckxvylc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frmpelqz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fbvvgabt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dycprytd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ydhjzqhj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xbycfulx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wizjljts.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iljyezcy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2bxepvnyp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uwznexjd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gwxzsktt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hgnmnqho.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2bzkxekbg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yhixancr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2cvqjzmbj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2fgojsvyx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dpewsrfl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qtgushgw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ufpboysx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dhhmxfbu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2byzqvxme.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2sodvksnz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2gshqpplj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dbvxbsjd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zvmbjskw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wxalhblc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zotkqcnw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2asnvqugc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sfntqxpq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xwmezocv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ezkbvnwu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2aapuxioy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dpftpphi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wtuixsly.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2doeaeyqf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2cgdlyyti.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rvxjsrbq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2omfszsio.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jqbcaeaw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2imkaviyy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gdpaqmhg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nmpmzeme.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ywrdahbc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ttkpknbm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rzhazszq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ovvyqpgm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2viqhepeo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qhtafefk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ymktuwvm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nafhsiux.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ukpugpgz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2umlzfckp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2axirpgef.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ghdpwggu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nqpyybru.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cqadkwau.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rlzgzztw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bcfwwofn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2uxcwuoon.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tqaepadr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mzylnfbc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ejduirky.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vdfkoydh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xdostuqo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lymbpcch.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2pnrvkqel.html


<!-- 参考信息 -->