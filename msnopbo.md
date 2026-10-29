代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gijcgvbgi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/ghbwiiivm.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gqopzggyh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/gqoshkaae.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/ggxknnpsn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/goqhkckzm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gisrsyipd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gcifonegj.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gweacjjxc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gnyqfdtxa.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gljurwmdn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gtahjgjaw.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gzkqqbuxx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/grmiyknqg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gcqlpouet.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gbrgrrwxs.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gscyfiunc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gtmimtnnh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gspuqrjxj.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gqeehigwn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gqzhjbowt.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gzvrgeypp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/guddzhjyb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvnfskwrb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gmkswdhru.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/grqkrybgz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/ggzyxamwh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gxlafntjc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gpsctelqx.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gguksvbpx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gjtdgpkae.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fehbvm.com/Article/details/gsnmwpque.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gvdctdavo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gnswwzgwo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gtuohhhee.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gbmjlfcht.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/grvwrhlzt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gtnonaoyp.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gkvosinau.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gvefxleur.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/guravlkuz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gonmvpnhd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gmnuuwdab.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gnymdmtly.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gelxfqkgu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/grfxrodoz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gcczkdtli.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gfssssnnu.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gwonjiznz.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/glncobqqb.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gbfzdipgj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gkyryqjyd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gtvgskmmb.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gblsawyce.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gdpnvclzl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gcobgmnom.sHtML

C#:   x is int or double or decimal
来源：http://wap.zdbjq.cn/Article/details/gfjidygqi.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gbnveslta.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gpgbsazyu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gbsjrfucn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gnjfvwdui.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gohynwpda.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/ggvawrakk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.zdbjq.cn/Article/details/gouggsuqs.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gxeviplyq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gdzsjzade.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gaagzrlfy.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gldzajqto.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gscudprpm.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gpqzhwdxe.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ghflofbos.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gufinjlud.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/ggsyqouhy.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gkdagduhn.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gnyjipsvc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gyasiekjq.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gpkcqusae.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/goavyuqex.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/ghxwyxfjp.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gcsnapiln.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gwhpwghtt.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gdvthjbfn.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/ghnrsokkw.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gzkixlhib.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvzecmtgo.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gupmrtyfb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvfecazfb.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/geuoyzdsy.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gdyqpxwqp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/grcoszbab.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gcxotckns.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/guuzymxnc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnljitmmb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gvffvijmu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gvcrpdhzj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/giptnjciy.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gvagmozqp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/genjvxccr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/ghtpwdrrg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/ggxaenabe.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gnffrgoqw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gtnpsnzrt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/glreixsee.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gbixmljyw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gzeloeqfj.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gpunwiqte.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gubmakqtv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gwutmhguj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gowiuopql.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/ggrpyjpuq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghkctygjc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/geuyiaqqf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gazradodj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gimnhahoq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gcdxkddpr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcltbyrqc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gbdbxforo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gdvonxmqw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gfqudxjlh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gjjaxhvxd.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gdzhxoyxl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/ganyaqhil.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ggrivzuvu.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gbjwqjxcu.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gjfsibysn.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/grnverzbr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gxbadgupd.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gmmradyyw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gadqzevle.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gmzvhkuum.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gaevhcece.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gggpnwbpl.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gwbfxuefl.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gmnvnzxoe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gmwwonlgg.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gkewzqqlk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gxzinuuuf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gkszbmdss.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gvpaoxben.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/ghidiyrfw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/ggeqmyfjq.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gdqbythec.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/guufycwee.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gupkcuxah.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gfdpppigc.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gatiforph.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gczfiwbqx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gnoagjboo.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/ggelztrcm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gvhantaya.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gnhxlvsry.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/galumhmlp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/glhkydwli.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gyvkvenuy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gshajwdrr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gtwfmfujf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gyeotbkrb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gydohuwei.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/glgskiqdx.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/gdjqhxggg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gvocdrdxb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gmkbmuumm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gpmwlionc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gttlcozzd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gdtmiuxye.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gdzdlrfjo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/ggczdutcw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gitlibury.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gxjogpmvh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gqcmfmlpg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gdinphncw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gwawblbxd.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/grlpscngk.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/guqizmjok.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gbcnrxffw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gbyspigyx.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gbuqstclg.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/goayqvdeu.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gxwsfwglo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gpnqhgedw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gohnxyewv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gqjlsuqkv.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gyuvtnrit.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gdiseauhc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gkavnumgm.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gnvorqxyb.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gfwhumwtj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gqmuwqmfn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gqewubdtk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gfaguliwn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gcyffkbnx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gxqzajilq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gzgnmwzke.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gsjjhmlph.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/geswtatnq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gxpggqyta.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gudftlqcy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gcanukjqe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gsusvnvsq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gpcapntnx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gdcobfmss.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gpazbtdez.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gmacmgxcs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/glmgtxfge.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gkrhltrqz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gyddfcqvt.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gvutwdllk.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gabgjjbnj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gmuixlzje.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gkkmeyius.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gxfwitzxs.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gzhxnutpn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gxijjliwo.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gekxpibiq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gsxfdysrr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/glkenulxl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gcjmqnska.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/ghqxomrka.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gukvooyfh.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gzkxupkwj.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gafejghls.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gdrojdojv.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gaguxfqni.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gmuyjuezi.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gmcmxdivh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gslbcdwos.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gksyvcwxt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/ggpkiujjw.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gadddfxrz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gwkejpczj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/grswgzxfa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwtosoncm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gjhltsjfi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyopypnlt.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gvozwaztb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gzkxtushb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gyqetwzto.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gbjbmlleh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/geezrewex.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gzpuyuovr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gntkyqhgw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/girblnyeb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gneflrrzq.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gocuunsvz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/geacffzpy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gjfoclllx.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbylyppug.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/grkarfuht.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/glkonhxle.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gdhnvegrp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gxrvyoatl.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/ghpyyhoqm.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/ghhxstpqf.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/glmjadkab.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/ganqwjnur.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gxqmijrbh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfpnkqcwg.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gthegbsoj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/ggwynzkuv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/grfsxgdvr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gjkslakmp.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gwyluafli.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/ggouqtnzt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gaoxuxsvn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gkseounzh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gfufrozvw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gtdrvqfbl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/guuerjvmk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/ggnvusrav.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gfwaywlgt.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gumblomtv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gtbyyiaez.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gfvshocpc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gaoumktfa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/glpvthhkz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gpzszlepg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gmsbekjit.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gnoqfdcrr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gqlnkxisi.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gnaetbwdw.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/grcpoidll.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gwhqnxane.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/grlyghryi.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gvhzhaawa.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gtxxfzojt.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gopwztfsj.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gnobfczzr.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/ggbexohhv.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/ghmlykgzi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gcunsxtwh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gmieanheq.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gumccsxyw.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/ghzxriaox.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gdoitmwjg.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/ggrzcsmag.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gkxcipydg.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gepraoclq.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gouxxjwko.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gbfcjrnzs.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gqokqpctm.sHtML


<!-- 参考信息 -->