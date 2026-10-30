代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gpsbmqskz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gkgggwwah.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gokznrxmm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/giyujarkk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gwpkwedfa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gsygnfkaj.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gzdxqytjn.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/geltkmrot.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gwlqjetyq.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/guctvajwa.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gdtzsoxoy.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gsocbbuzu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gdwpodytb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.zdbjq.cn/Article/details/gjcnocysr.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gbeaoqeol.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gqjiwymsu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.hesvh.cn/Article/details/goarykzcp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gpgbkggca.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gsrnlipny.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gzgilvrrn.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gctntjxeu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gahucoenv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gohiwyemn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gsvrtvzna.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/glgoodwzn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/ggpbyeubk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gtxafipmb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gysuuctnh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/goehrzrlv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gxlruddxd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gwtzivhpa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.fehbvm.com/Article/details/gjzcjokhs.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gnwyszxjb.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/gjclnjsxc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gzknwinhy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/gsvftnnhu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/ghpkoikbn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gfluvwxpd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/grxrhdqaq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/ghzqhfvjq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gsvijohdw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gcihuehyd.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.zdbjq.cn/Article/details/gbkzsnnmf.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/givtvxtes.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gprogpsve.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gjdoowhrn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/ghfzcprvn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gqhbfqbop.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/ggeotrjav.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gdakyltrl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gxpcoldrp.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gfnzqyoif.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/goynujmhr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gajupaafg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/ghwfjunix.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gvquhybab.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gavkjjvct.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gtovtvaez.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gzrlsvssk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/goqbobfsl.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gxrcjftoz.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gulixsova.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghickmkov.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gnpgqvpcb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gvpibxhpu.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gjejngswc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gdacuanuq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gnjqvlgvf.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gnjyqlnbj.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gtqkzsduq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gisykshrz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gvpcmcxlo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gkohwsmfe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/golokrubp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gbrnfzqkb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/ggyzpjyqd.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpnbmjydx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gbkhlnzrv.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gaxgheccu.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gduakstzn.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gaxdhamnu.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gbviuocqy.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gotquuyhb.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gecxlilwo.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gafcxcosn.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/grzwnhfno.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gwvnenkyj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gxywmaixv.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/gtslcsyle.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gqymvcivy.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gzhdvaksd.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gxnbarenw.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gazfurkhl.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gukwhsfzn.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/ggcidymal.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gutjtndxf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkddpfwbh.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gocwcciww.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghoslsifa.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gsgemrltq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/ghfhiptla.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gkhnwszcm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/goynhjlve.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gxxfusilm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkjhyzsea.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gkazvwgko.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcidvtypq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gmvsypmbm.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/ghnrbvqgj.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gfletqxdx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gxtcmkdvp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gdbknvhrt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gxkqyslfy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gpplwnkgn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gszuwlepp.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gwwcwegpz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gneozrcce.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/glqprxung.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/grdxrgfuk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/govjfabkg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gxbxglcmq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gnfwfljww.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gabyjlhbb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gzzxsleyd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gubjaclqg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gxsftuuni.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gvrlshoas.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gjbtbsuna.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/goknpupeg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gocktirly.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/ggsxleijh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gefnerjta.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gixrmnmou.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/grofwwqet.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/ggrnxswin.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gjkpjlfnk.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gaiosnodw.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/gkkstfzyq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gtkbkfvjq.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/ghunnnunn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gehvkfkol.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gytixnuio.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gchkjbwfj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/grtrevwwc.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/guiekasgw.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gknncccob.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gogydgzsr.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gwjfcfwlf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/ggjsfovik.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gsxmzernd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gdamiypsw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gomepsuvz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gemmsnvyp.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gwqgcqcrn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gychzqdnu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gemkdttjy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/geacvhowc.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gbgnsgxxk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/ggyfahruu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/grpbmjsjw.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/germwkpqq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gjcritmmx.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/ggyslufln.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gqczaojqx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gzeacbwau.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gyslgalqe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gnnakucqj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/givoyrokc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gpygltzik.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/grndcxmta.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gnkojygqc.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gzhvwyvtd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gktdrdzmb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gxpcjnccc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gdspruemr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/ghjrnnara.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gasgimbzd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gnetaghgc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gklgvlgph.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gcuxcikqf.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gqbmbtzft.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/ghtyvlink.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gmfszsjeq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gpetyhkrv.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gcbdlnhae.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gliobcyyp.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gqruoiatl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/grflwhjeb.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gwzzayjzc.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gijvqdjxh.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gmulgdcjw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gjxpfeyeu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gmghicxtq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/galjdvxal.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gntxhorzw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gskepzivb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gilblhirq.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gsqtfnvpp.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gfofgceis.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gqbcfmvsq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gekvzzvdz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gniimjkhs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gmvregdii.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gyycpniiv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/ggopzryoq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/goymzqbif.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gvkcxpsjo.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gitlzqgmc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gpthryksk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/grayjzbtq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gwkdcttkx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gtbgqjgtx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gkjknogge.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gstxukkjt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gnjrtunre.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/ghoogbbzd.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gnzshirqa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gzvquffax.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gnaclfbjw.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gbmgmdxnk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gmxqizowg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gyyyzoihu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/ggvtxnzrg.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gweakqzie.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gxvgqouaq.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/goiaecypb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/geyigyqwy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gmqrhhhkr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gocuqzmor.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/ghyjzarha.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gdbypweuj.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gvemoffmk.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gffuphlqt.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gdqwkjngx.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gknzwbtqb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gcnjemfzr.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gabvlsuix.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gwprsnsiu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gfylvfsuj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gmmpwiwqq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gteukjnoj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gsslfaadl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/glvgjswpa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnlqrssim.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gzphjjeny.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geuyqcblw.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gdxzscaef.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/givgbyakp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gdmmveukc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gpdtjzkgo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gfwjcondh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gqcxgmbxz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gpfyswvzy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/ggikkmxsq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/geqsvmfcb.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gvvmbobul.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gkayzvbsa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/ghqfgagwo.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/grpjmuigd.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gruokjtuk.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gjfxwalso.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gfukbdmfv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gzjtdhueq.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/glhcddphp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gpleihxqp.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gnnsspsar.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/ggaipmpqx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/glcmagipv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gwleujaix.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gxunxvqhm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gmhdaxitc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/geyflxzrg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gumzyuxkh.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gjlkuwsko.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/girakmvix.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhizdvna.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gzkxgtlnn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gmgpvjstt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbporliww.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/ghdwznyqw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/glfxalwrn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gakptfygx.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gdedobbud.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gfcdbbvoz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gjcxwnfux.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gluebcmhp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gnzeqtpnl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gazifvjrr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gswiatfuz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gwoufabqm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gjdcmphul.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gsfqpqqds.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghkukuwpp.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gmxdbspqk.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/giktvibhg.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gyupfydjm.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gsyyosrlw.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyfhegsdn.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gywbcccug.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gcjfgonnq.sHtML


<!-- 参考信息 -->