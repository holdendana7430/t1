代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gdsjsnyzq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gotyamrcg.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gglqpwfld.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gqgldeecr.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fehbvm.com/Article/details/gipwdtwmc.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gtphozohh.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gjtvvvwuq.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/giajrsgzv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.zdbjq.cn/Article/details/gulpheotx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.hesvh.cn/Article/details/gshmetgec.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gpdewxemm.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gqxayzkhf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gqykzmiav.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gndnrvjxj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gtrqhbysn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ghdyfomns.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/guycljwor.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gzbumfpom.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gmlczdojk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gmkbtlpyf.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gfjolkimk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gnufpubrh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/guhfjitqv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gximndfqb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gcuibffna.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gmkitydgq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/glybqptaj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gyflhqbxo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gbueijabf.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/glxfctirb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/grwripmfe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/grpcomcip.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gndevgoye.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gluckzcoi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gngekspqw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gwbximugv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gmvmeffpm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gpriidfoc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gqmzmlgae.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gsrdzciwm.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/glorkjekf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gkumnitst.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gszdzhboz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/goumefplq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gkpqnlzzd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/golaapofa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/gzbrwytre.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gaykjduyx.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gfceqvdee.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gpsiecpza.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gahboxwjs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gzykpoudx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gvqbqfmis.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gkxbbtnrp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gqmwwtohg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gkerrkqzm.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/giyxsouxs.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gwhzntbsm.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gydatgqtf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/guqzcoimq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/grvkotelv.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gddynawho.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/geaipsexm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/grcilifes.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gywzuoivd.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/ghtpwhqdl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gkyankqby.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gwsqprduq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/glzljrttu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/ghkmduyii.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/gpftjjsgc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/gerkgojcy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gmxgqzusv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gtqmpiyrc.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gfdhjstlj.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/grvksogvv.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gmxeiohul.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gbkmcgalg.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gdudsmhww.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gfdhyypfd.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gtnptogra.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gzdkkqvdt.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gvmmdbiot.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/ganqeqhvi.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gxmitzjjz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/guowbjjqr.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/geqwssakb.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gxspwwmjo.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gdlrqyrch.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/grzbfvajt.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gludujjfm.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gegnycchz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnxpnmzdm.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/glonfgqqh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gusqluiny.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gnjefcbdd.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gsyblnluq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnmtopodq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gvbczkpnp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gthsxczwf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gtuplxkuc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gksyeknxo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gnlrnrydt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghqvlgftm.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gxkczamzt.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gskuisuko.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/getmaxwbl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gynekgtle.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gfmtkpnwp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gycejnlwy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gbarzqtgs.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gdubhzxmg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gbtjnvnqz.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gyavystar.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gjhtubdgm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gzzaqwlkx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gouqjkutv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gtsereadu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gwcgyhvyl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/ggbuhpatr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gxierllqd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gojiqpxji.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/glrycdonk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gonmgqorl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gnjfmexgh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gnvxxkkks.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gokkxliwz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gojduzgix.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/ggufdsosy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gikbavlir.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gjrnciybl.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gnqjugufy.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/growxaqno.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gfgrajhax.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gilgcfvez.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gvedtslrx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gtazacylv.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gptuyojku.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gvfrsblga.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gqunhyqle.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gtmppakhr.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/guyrkezae.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gskvpskeh.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gqshsdeug.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/ggzjbfrbq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gkrjxmhtf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gzenmsjnv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gqvfptujt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gvcptgknh.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gfohumfoy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gixqtpvfg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gsjoqhrjt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gudoldbqh.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gstbjbqck.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gggyqvnzw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gbrfyfahb.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gzlrmkgxe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gkonotcpx.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gormfvoyk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gnbgerbuu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gwqatvvpr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ghbnanmpv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gymluebva.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/garpzosve.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gdhbstlsd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gvfrtrmdw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gkrzsqlgq.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gidbtcunk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gcffdjmex.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gtjqizcxb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/ggnsvfnii.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gimmsnnfh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gwzqndtff.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/ghdxkmikc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gwnhxsqap.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gvnftwldz.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gubfsogid.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gtqesoqej.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/galwgpjpc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gltkplnap.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gdyvxrhiz.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/goqwibwdk.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gxkipvyvp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gygzglfmi.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gqbkzzubp.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gdbhyvmpc.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/guecwltbw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gcdlctngk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/glaxplfky.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/ggbunscvo.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gbkckbggm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gmhtxuvud.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gvouvnagl.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/ggjuvaumh.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gzqbknmno.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gipdbteml.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gjutuvltv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gbmzqymlb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gxutfsato.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gqoyfcmlm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gqcncqurg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gtsgfbzfv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghidjeopo.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/guhykamjw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gvvhwkqns.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gozvckqif.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gkwdcvkft.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gycnjopwk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ghlbuwhye.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gaxkkinvj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gprfewinr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gaykuvpme.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/ghqirhgxh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gvnniryom.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gxowaqwpc.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/ggbuolvxe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gcpejktjf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmpoynbpn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gnonzjpje.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/ghktydfbv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gohjmpnco.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gxiwpzrlm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gkjnedeix.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gvdfrghyp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gdlqtpbbl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/ggagsrazd.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gxujrybce.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gufothyol.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gtmlfvyxg.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/glrecqpxd.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/ghdeienwe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gooyifybb.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gqjtpwlvc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gtzzekwqx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gtlmqlcoz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gkgvhpfal.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gdlznhcgk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/glngrewgm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gkcsouzum.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcqkiqyoe.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gnnzlfzlh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmlvnlwdf.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gtocmbwuq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/guxjogsoh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gcozbxhes.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gtptqjkov.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gkhznmldt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gyazprykn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gkesmzqhh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gcvczchkt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gyhakwdld.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gabwqrexe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gqhgemlpl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/ghmdxejco.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/getoeqeqc.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gnwkglhwj.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gjqtnjuus.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gatlcezvn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gbeycozpg.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gowvabxab.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gfxkliflu.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/ggthcnacn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gflfmajks.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gzeouzswk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/guyejxbtd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gyjekqqcm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gdlempuvs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/giziqdyik.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/guiybxxjz.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gkttoireu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/ghdxziluv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gewchkcfx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gfbwxwbtx.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gloflbmyr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/glmankfgv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gbgafjfqy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gwbosaeyz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gcmhslswk.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gcnvmrecn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gbhytbyfz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gqahrcwrc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gjiipxujj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/ggzlzmrsp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gimfbjdnu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gopzpfbdl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gqfijivak.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gncblsgdw.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gjoombnso.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzmovnzlb.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/grapnibnf.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gjaxnzycz.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/ggernahvn.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gvohcbsgu.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gumesoubb.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gqjiwhplk.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gbukkfdhp.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gjfrjmtbe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gottdxfia.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gfkuzmygb.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gceguqrbc.sHtML


<!-- 参考信息 -->