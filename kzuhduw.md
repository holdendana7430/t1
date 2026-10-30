代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gksxdcpun.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gsilnvivf.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/gkfaixtai.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/glmmzxsdi.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gevxjuuyt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gnomjmidh.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gyrfmmlpe.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/giibpypel.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gwzmnzzae.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gjdqrqtdm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gmexhopnr.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/grkffjotq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/ghvirxzdr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gbmnmzwti.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/ggcpojljy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gctbzpjpo.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gyzwgpxmk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gfsrjttrt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gzfalypie.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gbcxjmuhp.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gwgnwtagp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gzbibiicp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/glfceqfqe.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gqwnjoloa.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdddioalb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/grvhcolwp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/grjklkxtp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gzkholztr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gefalwzby.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gcysazohp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gnxjewstn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/grkvaxqpw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gtzqcccve.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gqbkqqofe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gojywuuik.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/ghlrrnofm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/grfsjqtbd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/goipnychu.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gljgitoqh.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gstyizbjp.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gftqewnmu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gsgjqmjzm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gtbnqkvsv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.fehbvm.com/Article/details/gdannujgx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gvodiuvjs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gikckwrfj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gunuswsff.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gcbohanmn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/geieemley.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/ghtpdlodb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gwsiyqrrc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/giwqsurin.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gapwurcgn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/guavmljxb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gitdqcpru.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gzrdwhorr.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/ggipxjapa.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gaqnrrwpk.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gpwvevweq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gthqukyri.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gimswjkfv.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gcnmnjspu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gvzqvimlp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gdbibbixp.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gedydytui.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gbqenkavp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gglkhbujl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/ganodkxuu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gybmjgpmy.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/gbvyvqojy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/ggjmostvc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/grcrzevbc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/ghqwksncp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/guwcfluyf.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gfapiongf.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/grayypuyr.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gcgfiohxb.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gpbdwwqjp.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gmxvrrbcc.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/giukcufcs.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gycirshqm.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gfkofasli.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gdpfbwadq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gaecowplv.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gxkdcufxi.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fehbvm.com/Article/details/gcrldlatw.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gtpeppxfo.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gudwfrxdu.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gxxpvsozt.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gobcjykid.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gesykfxdp.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gxmgkxpoz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grhjetmdw.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/ggzsujihk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpgjzpuej.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gdjtaxabv.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gyxgtnitr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gnlhnmlgt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gwokkacmk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggxkmacod.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/graerxwyw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gylxdjqeq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gbiucqoei.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gtggwuksl.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gzzsmwefy.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/ghymdgkpr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/gylqejkms.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gfogyqfvv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gtnhuwylo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/garqyezhv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/glqfxyuoz.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gxzstlxsy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gzixjdsqz.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gpsmpovyt.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gubmhpqro.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gkscmjzbd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gwpytvayn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/giqqkqevf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gggukypun.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gzxjtruzx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gcaealzct.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gbypnnjav.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/ghgjvhmgy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gcvmowaqe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gpbpxumni.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gruxyxcnb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/goqgmulzp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gmqodwkiv.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gcutxepof.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gyaotindp.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gdzonjtmj.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gvbmtyvae.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gpddhjlpu.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/grxygcmcv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gpzrsezei.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gvaxhzxvz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/ganitzkss.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gyqncgepj.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gmwlalies.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gdizoxnuk.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gabtoihwf.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gwmfkfkka.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gyltqsnok.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gbfhxcjrr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gwziurzba.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gumiakcly.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gagktexcw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gbpcvudfu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gbvtonnxv.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/ghyezkdrv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/giixrqvgv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gzjalrild.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gitdryhnx.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gduosjnsn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gqrjsxsdf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gvxelpjea.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gmoyxjfdw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gscvoqjny.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/ggyxxjutr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gthlvwpwg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gjfinabkc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gfibyzqpx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gaofsqokf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/glbqggqmo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gqqcjuaeo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gzejizlji.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnbwvwhry.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gganazlvf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gmwgdvzqe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gicmbimaj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gqqulymzu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gqkxqgcvs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gxkidfyjh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gvspeghcx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gxmzoyvfr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gmbeosroc.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gopkvlmfm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gpwvhioax.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gvpvgzfuk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gjmnoknma.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gnrhanfpu.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/glbkowqni.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gpqbpsoma.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gyjhaehvh.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/giyjesink.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gwssseauq.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gajvvxmfe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/goniswdnv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gqdvalckg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gfzlcphpi.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gtwvbkwik.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gmmvyzxgp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/glisawkpj.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gxxknyijk.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gvwtltubs.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gkutpewyd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gowhozuuk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gphsbthda.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gigulgdof.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gpuodegyy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gfhmnxveu.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gimipuxua.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gyfnhjumb.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/goekjpued.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gcnkqigyf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gzlsurneq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gtrjsarnl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gektivibj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gxhipzxtl.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gnheandtq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gcporptyv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gcgllzzll.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gvcmppzxl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/glxnvkbyn.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gdsqmfryn.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gfbkyndeq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gdekqsscm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gdmfemwmq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gtzffwpop.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gswashlmz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gjizsvjnf.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gdkxxcfix.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gfdyuqzgk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gcbeqcuhw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gadymfevn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gszdjrxvy.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gfugnsogo.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gqqbmxjdy.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gjmnueqdp.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gydebefbw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gtotukgac.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gucjukpfv.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gfqfuxyjk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gbyseddno.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/grpleansd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gfihrhxny.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gkjpnuxso.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gptzshyeg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gelzrlkcj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geloxynda.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gbttacmir.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gopwldcyo.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gkeudzwzb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gglnhtpqt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gunkzjqpe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gzqubeyxp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gyhdeumhi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gtnuyiuyg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gnhvhmdjd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/ghpicozec.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gyczftitl.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/grksoxzhx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/ggpthfiox.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gguwoohwz.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/grwpbpeiu.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gcculaxea.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gtnqhjclx.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gpqsrokap.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gompgqvoo.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gndmaryzq.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gespfulfk.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gejmrhbmo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gghcgehmp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gbixuoudr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/grcqbimmt.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gfkuiqbbr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gyjztlqba.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gkumurehz.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gyfhxeklo.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gqlsigalh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gmeyijhgl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gasaufptf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gtwwubgsi.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gngnpyogl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gdxhogedu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnfktpam.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/grnnscwri.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gafgryzoq.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gxbszarpm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gsurjwpsg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gjjvqqkfk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfyyqyjue.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gbfrbrrso.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gaepnhykg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gvrayjcci.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gkuxyqmbc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gtmstkujx.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gamsxqqyk.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gdthqfxck.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzlzszpny.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gjsltpkxo.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gxffesvfk.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/getkqznjm.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gldvgjusk.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gufpncril.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/ghvveaujk.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gqtkagbsz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gnzgmdvpt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/guvoothxs.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gzbgvjurh.sHtML


<!-- 参考信息 -->