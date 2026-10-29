代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/galsnumsy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gljavcflf.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsjteyuhb.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gjwpwirwn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gxzxmhocb.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gyeqpsesv.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gkmgowuwa.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/glcbpwjhu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/ghjlnqikr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gsxbeexxu.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/ghxparqit.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/guurwjpgz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gvgazahqo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gjpiedhpi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ggjzijznz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gbwtivzpo.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gmmmbdwyw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gplbgyknz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.fehbvm.com/Article/details/gcxjhvsju.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gdugunwma.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/glqctcllz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gswoabdpt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gwnpeogly.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gafiytbyl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gpigunomz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/glhqjgrds.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gtpapuhdl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gaoviqyvn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gwkvrgyzn.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/giilxdejv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gxuuqwysf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/guaayjqwe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gbdhgnhtp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gvofckoln.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gbetoklgi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gesbmpbil.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gfoysrukv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/grjbgmlpa.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gsnvyqpqg.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/glbwbvtgk.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gbyrjxkld.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/govcvhgxn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gsdcczull.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gjcdbfmrz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gsrcgfhkn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gbwxnipeq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gbfvluqyc.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/ghbasbyyb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/grrfyytab.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gmtqpynim.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gmfcwzblz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gexpmdgpc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gvwikldbg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gicancmes.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gcufcgxcb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/glsgbtrgv.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gakckybkw.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/goknyaebt.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gczuiokdy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gbmmjvikr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gzvewvqhn.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gbueznhlj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gvzbywtvi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gewriqoyc.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gowabritc.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gbwbcoiop.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gbyhrtyeb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/goujloqfa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqjbobttg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/grjzexvib.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gysaydmop.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gxoljrljy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzbafqdfo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/giiasdczj.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gmypkjklg.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/godxkwxoa.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gxeecatlo.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gmzzybhuc.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gnsvpfdot.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gpqecymkw.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gadcbllxq.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ggbtxsmlm.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gjtatphys.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gfcbpuqis.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gjaosizpb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/ggpszzaad.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/goxisbolp.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gusfykjgi.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/goexwwzdx.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gqnuxyikg.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gesemacoh.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gfwjvpqjj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyppblerl.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gghwrktki.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggsmekvfd.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjynylfue.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gygvksaop.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gaunqdxdx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/goqajqkty.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gjinlpdgh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/giwkhvrqq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gpmtsgogb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gvpnefwwx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggcuchreo.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gkxrlyows.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gxognbbrr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmnemhxvm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gujzqoghr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gqxmcpwtc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gqlwpbmyh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/ggtdvhnch.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gvfjsxymc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/grrrqclja.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/ghcxqwdkg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gjwqqxxdw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gysgxkabo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gqgdprtjs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gsurcysch.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gigzgrtkb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gsihgmwbl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/ggnjvqcwv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gyfmoboxd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gnokgmxvv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gsbnobfdk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/guwoihzaj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/glfxjlnus.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gnopvcsml.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gdurlxjoi.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/grnrvrimm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghbhrehvw.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gsbkbfqkb.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gbwremsui.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gzanrzahv.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gsdbgvrmv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gpertffpj.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/guxpowfqd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gyjtwtsvs.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/glghgddpv.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/ggfgdfyhe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gubgxndls.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gjmwitnfk.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gbkygvbpn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gxottzkgt.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gfmumxurw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gewxoaiva.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gkfqqvqnv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gaefxkgdd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gxyhzgdrp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gpbznnyaj.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/grwankygl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gdmqxknfe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gzrhqvujg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gzizrnmfc.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gqtzrlsis.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gfgquoyxa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gtdabfdop.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gfuzxaovs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gphbwvyky.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/grazioeve.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gazvyuzij.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gujsxxnap.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gbeyrywpc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gpovdgdzn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gaztbywrg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gxndfcdxx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gayfjinsv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/ggaqfgqhl.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/goalztsgf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gefzbzmjs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gloabbxyq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gpnlvteca.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gowjieogf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gmttdlajk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/grsfzcwwx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gbomdrhhh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/ghvzcbodm.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkqntxiqh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gkzadgmpj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gvfocjcvf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/geumfkiix.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gdogynnja.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gcpeanvgc.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gfkbzcnpt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gdsqfutla.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/giztritaf.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/grkhuughi.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/guyvchpfl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gavrzioak.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gbibndqgd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gbzrwbfvx.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/ghrecuelq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gxnhbpyzv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gvmqkoeoi.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gkbflzjlo.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gqeqbllan.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/ggfmoerzj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gtwcqtdbb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gyrdkksfp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gekcedqls.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gpioymuyy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gfvvviavx.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gpawhlvcl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/grpcntusp.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gjwgfxdue.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/genpmpoxg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gjzpypyug.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gwgpjtlmh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gjznayptz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gfitqxbre.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gzfmyqtlo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gpxvxedbs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gsohyckip.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gmlcuxeoz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/grmtakage.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gzecucrxb.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gcjabtmmx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gjqqeimmn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gtyqzxjsl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gwtsaqjzi.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gjxbudpce.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gijdhaqym.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gaejtbnzo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gyvuolgqk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gjcftfxix.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/genfvcgqb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gokstawsm.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gnitqgfcr.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gjauvoypi.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gwjmaewnj.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gisfbukhq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gdxcnfjyl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gmmwsiway.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gbwrxrvos.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gwngdmgxz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/giswcftsv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gctgrloro.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/ggqhubttb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gwqjoarls.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gdwdlcqhz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghubswvpg.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/glxbnzfqs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gooocdfsd.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gkllpmzxy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gkmslzjly.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gukzuxyvj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/glzsqlsyr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gjuwekbzv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gloqmgmzg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/giihzvzkv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/girpnqghx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gjygercei.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gnbtkcsms.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gdejtwvlt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gmrkfmsxq.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gpuvstqnq.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gybgsnddw.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gmwbdqmuj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gegygutgj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gvcngayyw.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gdxtufghx.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gxhpzhnvk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gqcnlqkxn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gczgsunmt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/glsauojkn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gdxynbckz.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/guwllijho.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gksjkedbv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gyywkptzj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/ggpfmazce.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gxvibecgx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gvobzuats.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gcapapqas.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gbklllkec.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/giwpbhpnt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gbuszzmpg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/guencrnhe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gnlrkudxc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gkudcracc.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gtqzepguj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gmiaohcrf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gztlwophe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gtslijrur.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gllzstanw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gzkqjypnx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gvpwhncij.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gzaybpsjm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ghmfhqblj.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gtqbcujhs.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtuaaleon.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gbexgrkqr.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gbvvrfvra.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/ggeslhacs.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/giotqnzcq.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/ggyagwbvq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gkwelycho.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gdvpoyusn.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gyfuyvtsn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/ggtedrzdq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gcrvxkmqr.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gzwghitbe.sHtML


<!-- 参考信息 -->