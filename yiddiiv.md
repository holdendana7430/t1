代发 wailian999

[B09] break 与 continue
来源：http://m.share.fanxiaobao.xyz/Article/details/gidkdztrg.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcivvnhdt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfrpfoqb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchkroryl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gubwsrrwq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgefntld.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzutrotvs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fanxiaobao.xyz/Article/details/guctetjqc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuwumuix.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gcvokcugg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfalkpam.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkyezkjti.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gjbfsfsgh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerzoikwa.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiahngvb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqihfzpji.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fanxiaobao.xyz/Article/details/gcutmfsfi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfuwavqd.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fanxiaobao.xyz/Article/details/ghsyoxowg.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvezpybqu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaigoqfuk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/grcugrzyo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwfxdfpu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyupxwcp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fanxiaobao.xyz/Article/details/gmojmlmuh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/grqqfepko.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/ggjohaoln.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaicoytjp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/guootdgat.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gghgncrpv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gmdteforz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylcogxoq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhmpvfch.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiorggyp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gowijwwah.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmriumawg.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/gwnvphzit.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqddizto.sHtML

PHP:  is_numeric($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gvheyypgz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnicexdpy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghourawkf.sHtML

Java: x instanceof Number
来源：http://wap.fanxiaobao.xyz/Article/details/gbyarwewh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gotuzsuqc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fanxiaobao.xyz/Article/details/groewhiri.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gizifupau.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fanxiaobao.xyz/Article/details/gnwpwqjoe.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkxotmol.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrdvvnpd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gzpltqrrf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gfnlvxdmn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwjdrqbt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswmtwcuj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuzhjeej.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamlxvecf.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgsfauol.sHtML

Py:   a and b or not c
来源：http://3g.fanxiaobao.xyz/Article/details/genlhiwkh.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fanxiaobao.xyz/Article/details/gktnklctr.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkygrluy.sHtML

TS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjwegndd.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghffymzpf.sHtML

Go:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gspltdmos.sHtML

Ruby: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsodgepi.sHtML

C#:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/goubnkcpr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcxpsxfi.sHtML

Py:   if not data: return
来源：http://3g.fanxiaobao.xyz/Article/details/gvtliibsh.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnupsuhzv.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgqxoxhx.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gaxgsrzfd.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrcjnhxx.sHtML

Go:   if data == nil { return }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjkemutz.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/gaqaqwrfk.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsylwiduj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkagdefvy.sHtML

C. 函数与作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gshatbfcj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gaadsnlqm.sHtML

[C01] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfcyverj.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gtbnzkvvj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbivhcdw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/galwfaprp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjnhnhmiw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfrsbexmg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gitfiqboc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gxobkbary.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdpaxmhid.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepwtlvbi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gcknahbqu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gerqivxpw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucgwfbpc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsattuorq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fanxiaobao.xyz/Article/details/ggofoszxd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtieldtrp.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/gxbjhdchq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fanxiaobao.xyz/Article/details/grbbvkadh.sHtML

[C03] 可变参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvqnkhnq.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gfywladko.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfunmeueu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvrvjbddx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsytnhwdx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsodxzjt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxgzagri.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fanxiaobao.xyz/Article/details/gfhikraqj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchwnwjrx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwuntthy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvepnctiu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbabptcck.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggbhgzisj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gqbjixeal.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fanxiaobao.xyz/Article/details/gkwrnrree.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gqohcfmxm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvbiririk.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/guxxrtixs.sHtML

[C05] 返回多个值
来源：http://baike.fanxiaobao.xyz/Article/details/gmhyidsdv.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewsykozu.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/goxhzvtgt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gyebdtqjx.sHtML

TS:   return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gxbuarxbv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/gwdnszusu.sHtML

Go:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqnemaqv.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqllvcoj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fanxiaobao.xyz/Article/details/gijzdkrxl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigqvicxs.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fanxiaobao.xyz/Article/details/glzgrzddf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbiuooqy.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/glaohzexh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gfwlyoclk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrcrfrrl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gjnkznrpc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gcsugugwt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gydbvgyej.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtzjlamk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fanxiaobao.xyz/Article/details/gaotmjcqw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gybxemnqx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/gwdbdkbqd.sHtML

TS:   arr.map(String)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcdkxdxn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gwfovxitv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fanxiaobao.xyz/Article/details/gsoqkldrk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmybgjbpv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnarvghbr.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvazgngv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fanxiaobao.xyz/Article/details/gdhptsyhz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gafjfufbu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbowywcmq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggclwpfzm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/gcqhftglz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoiwylbb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxgffzec.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghcrpfzdx.sHtML

[C09] 递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhiijdlf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdhmiojw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gendavezg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gdjoxoups.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gwwxcsqmd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxferzvdh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxemsfoo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gasgxmmwu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsemxhdv.sHtML

[C10] 变量作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbguwgwh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzevyyby.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fanxiaobao.xyz/Article/details/gqgigdhvt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/glpcnhvko.sHtML

TS:   同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqizwkwb.sHtML

Java: 方法内为块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gpbjpsyxv.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gayvtdpjj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fanxiaobao.xyz/Article/details/gnfmcshjm.sHtML

C#:   块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gklebxgby.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtckodxod.sHtML

Py:   from module import func
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcbphniq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmgdtfrz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gpfemlqxx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/grwpnauqh.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxyehhrk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fanxiaobao.xyz/Article/details/gzsbywnwa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaegxpmt.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmciboqfb.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/ggeluqwne.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fanxiaobao.xyz/Article/details/gfdijahug.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwnvufud.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjejdsfkz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkykdnkb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbrqdqdg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fanxiaobao.xyz/Article/details/govjcvmjd.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoobdnaq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgclwoaj.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fanxiaobao.xyz/Article/details/ghhypyrkv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbdavwnk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjlyrcwp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fanxiaobao.xyz/Article/details/gehhkkujl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gujzswgsa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbigjvcr.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvucgjqq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkleyeidf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fanxiaobao.xyz/Article/details/gcrrehecc.sHtML

[C14] 泛型函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyomvoiyc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcibibse.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gvpfcnsdm.sHtML

JS:   // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyymmgsn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkallimxs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gohnbvdvm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fanxiaobao.xyz/Article/details/grsszyfhe.sHtML

Ruby: # 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/govazyzvb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbuvsibp.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkyeyarp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwrqzybx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcnvtzqc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbsxhkay.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gadetquyk.sHtML

Java: // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/gjucvmvjz.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/giiufgftb.sHtML

Ruby: a, b = pair
来源：http://baike.fanxiaobao.xyz/Article/details/gzkjqhaqc.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fanxiaobao.xyz/Article/details/guxuprcsr.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gzadroeka.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/giwxhnvlh.sHtML

PHP:  // 无重载
来源：http://m.share.fanxiaobao.xyz/Article/details/goqnwkldp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gixctlsiy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeblmtxz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdklyorfj.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fanxiaobao.xyz/Article/details/ghtbmhogg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqcmglro.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqeafbgw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gzttvbcnj.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fanxiaobao.xyz/Article/details/gbklizbpo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqibtwqx.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gxiouzqve.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fanxiaobao.xyz/Article/details/gbllyiduh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giypovoil.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/girulqegq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fanxiaobao.xyz/Article/details/gbfwnrvbp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fanxiaobao.xyz/Article/details/gtldvjvzz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjatzyve.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllmcokye.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greoyibch.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxvmrwbl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzavoqic.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/gfikdyszr.sHtML

JS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzihylqvp.sHtML

TS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbrtyzzv.sHtML

Java: list.add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/grubiroqh.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/goskidzfd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdipsnjlb.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gpfjgvssn.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewmpxyeg.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gonbhsmzh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhqghdpa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fanxiaobao.xyz/Article/details/gjppqhzys.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecshkios.sHtML

Java: list.add(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gwflboqqa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gjolazoyt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gingcuhjd.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gypctkumt.sHtML

[D04] 删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/guwtenmxf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmaqpqay.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/ginkuzfqu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbeouabx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqqdofqb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwkmtmxf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fanxiaobao.xyz/Article/details/geydnxdff.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/guvqjipck.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfskbezv.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/gjfzamstb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbtjsxcf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gursjsyrt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/glmevopnh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzspbfkq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gswkooitr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gegxmcnpf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gziymgmve.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjdujysi.sHtML

[D06] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gniuxqceg.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gvnbnkxez.sHtML

PHP:  count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyicykdc.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/goetacezn.sHtML

TS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuhhblso.sHtML

Java: list.size();
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbfyrirj.sHtML

Go:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gazzrceeu.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gppqbuqjt.sHtML

C#:   list.Count;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlvqdves.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fanxiaobao.xyz/Article/details/gywlxkvyz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fanxiaobao.xyz/Article/details/glftrwiyx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmdrwcxeb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gelacnamo.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvfimfdw.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwohklsmm.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/gelwkzmfe.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlwngxfo.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gewizylvk.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmwbyulw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gplbiggfn.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxjuuaak.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtzzcxny.sHtML

TS:   [...a, ...b];
来源：http://wap.fanxiaobao.xyz/Article/details/gojrntvkq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gspbkjizq.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/gctszqetu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gdvzailnn.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/giiamudkq.sHtML

[D09] 排序（升序）
来源：http://blog.fanxiaobao.xyz/Article/details/gssnenzfq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsacqvoc.sHtML

PHP:  sort($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gwrrfzdeg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fanxiaobao.xyz/Article/details/gqemmwjnz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geexcmymz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gntxprppm.sHtML


<!-- 参考信息 -->