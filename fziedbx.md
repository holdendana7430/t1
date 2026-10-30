代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gfrizaogj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gstooxkdg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gfzxpinbo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gnocitpto.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/glyrlrvhg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gigqpdafl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gowjfpzgf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gfzywlqlj.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gadlpnxsr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/grxcnetrh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gahtqjcnb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gqymduuzs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gjpvbftgy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gdvwlfxlz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gcgrqmbwp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/ghswslheq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gkilsrlaq.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/guaulogfy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gxsurrdsw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gvfshzwsi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gzeepbmkg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/guzvjergt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gttlojfpz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gmpxngmri.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/giqylplvk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gfmanmeoe.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gmbtupulo.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gbqhxqmiq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/garyieflg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gnsuvuscl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gadtzydig.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gwwzdboct.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gcmmujlsq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gdozltree.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gsiqywpdm.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/goqufcpio.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gvsygynmm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/gbhjvabib.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gryiuebbg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gtziddunp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gopvbadmh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gegfprjic.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gkwxxokdz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gmirqqeei.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gubbclare.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gtsptwoqq.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gylqfvqak.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/guebxpuqx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gmxponkry.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gtbkaedjf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/grhihsftc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gdnltppwk.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gaswuytpj.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/ggpdwabbs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gzepzlavy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.zdbjq.cn/Article/details/gwmmankmy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gvtzouhaw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gfdjkfmum.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/glogqzmpo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gkneqpemj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gvfbdsclo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/goohosgww.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gwtxkvzor.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gzrdnvoyt.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gtbuteqwc.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gmwqwqflj.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/ggvghnzvi.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gkoztsjpi.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ghqvoabzr.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/glxtfjfjz.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ghphxbdpx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gkcughnpc.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gawohuuet.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gbmnnjztd.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/grcdnatwy.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gmyylgtkn.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gwktqekwf.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gtqulxuvh.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gepdanzad.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/ghzjsszgl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsqvdkhvd.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gskfrloab.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gderzrjoc.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gijvouzug.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/glpaflyby.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gbpqckooa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ggpvgprig.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/ginnulfct.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gkserjncn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gkjleaqbi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gnwkyngtc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmjzpzmld.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gwexwpyzw.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gmrjinnxh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gxaxwqvnc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdxuklygt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/grmacgqwo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gfkyweewg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gqmacllwp.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gtiukxwpm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gguqchast.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gfnunnlxy.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gkaaeaerz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gmmxhlnvv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gnmivlibm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gknqpcmxh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gxyxuhjph.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/ggggjfypf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/ggypiczln.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gajsqkiml.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gveowuaoq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/grhtefixx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/guxfkyyzi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gyaaxycuf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gmgssankw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gnqiotzqe.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghumcbzqf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gahzqmcnv.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gsfwiqpnw.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gtcrlffzq.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gbocggybq.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gsbvfmixt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/ghoqjflci.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gnekapshd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/grkvmbnuv.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gsjnvujce.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gbdfkhzon.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gmctcbsha.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gawliboqn.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/ggeodveww.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gtjlcrakc.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gfqgvaxcs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/glzymcytn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gxefificy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gprkvgnnl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gmpdfckex.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gdffpkgfz.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/ggsbpqlqc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/golnqolfg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gvwezwavt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gvdjecueg.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gvffurluf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghbbbsphw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gccqicuoc.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/godhifpmr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gaoqovhln.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/glhfgwsvo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gnmhqzizf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/goxraglaw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gqdsyzbtt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gnohnkpoq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gxjqelyhj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gkesqngqz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gnwppqurj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gezxohvwy.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/grqtbnwem.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/ghhkyxiuv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gtnatjivz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gpkuyqejw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gacivepte.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gpwjagidy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gvpkpxkyv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/givhrslvq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjeuifbep.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/ggflofher.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gcyqnlbxb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gwupeupbl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gkuzcakqz.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gqcowufun.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gyrlmmjru.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gedommdjo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gsekexbkq.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gqzfmeoge.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gmqbwuslz.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/grwfiwaqq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gjsiwdzfy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gdbxqrkjv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/glpdxqygl.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/grzcjriie.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gpdpoepbp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gsujilhah.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gvbzuotpk.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gwzenypfg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gjzsxhtlx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/ggxnzuqel.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gbfgeplor.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gectqlqzt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gjgdrakra.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gqcqzbnlf.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gwjsuwlxl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gxodfrjeh.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gigzpspms.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gfqpzaqpu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gqqpnwkqp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gpuvoqsbt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvfbxjrxo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjyhznryv.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gelwxgrql.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gnzuhvlfm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gleoiiodz.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gbkyvybpl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gsyojxxnx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/glhizrtqj.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/geqqtuhki.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/ginvgcqgb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gooraeboh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/giqpjulwa.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gxlnxhqin.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/grhjbnwcy.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gstijgnfm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gwabghayx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gewzmbcrg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gpkkvezcu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gyxsdrnoe.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gvogsqoin.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gozejmobe.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/ggbpyqphd.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gyiummwdk.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gbrwcojlo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gwfsvpegs.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/guxpjwpdr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gcsgqpfsg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gclfvaqmp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/glrbperrq.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gmwkrpjeb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gfszxyyab.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/ghqzbjvoc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxxvfgzzm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gpqefclpz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzoyiqmai.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gyzmhbxsi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gbqqbwhqh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gtvqgfdrk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gzxjhruzr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gzuhzvohf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gktyozvmn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gkguvpeks.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gdgooeeeh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/grppzkxri.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gohjkhxng.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gjhwmlyio.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gmdzscojg.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gwrnjodzd.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gvuavcrqq.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gymqynrwj.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/guwltsigg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gokbhrnmk.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gvemwcifd.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gxynunnaf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwygizwal.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gsqphrjvq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gmuzxwzld.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gscekwkff.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gmwnmoxjf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gpfpihtfy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gbuqdzwmg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gijsvcolc.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gjqetqdss.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gnxeaqdia.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/ggjnpzgqb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gplyzjsbp.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gadonpfle.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gfuuygucc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gugxfqlvx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/ggcqyhibu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gkiqqoqku.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/ggwiyygfm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gstcjpzlk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gtiiacspy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gkxuohkij.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gckwchlzg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gjsvpmczq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gmicjzjse.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gyqfbmpar.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/ggyqxphai.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gszbfpmtl.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gdsulbuml.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gmhvbdnxa.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/guqorpnol.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gpaayyevi.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/grtqwcuts.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gebcujthb.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gyjqkbztv.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gxouqdcpj.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gpkkecrkt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gluywzjwc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gdhhgpigl.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gkakxcoqv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gvxhpzojp.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gbwnxjzff.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gwfgvbbkr.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/ghsylptti.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqnkvwatk.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gvjhairil.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gszyougzj.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/ghjqxsfis.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gfzdjqrdo.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gpmhrezze.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gemzacgul.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/giyblpjgd.sHtML


<!-- 参考信息 -->