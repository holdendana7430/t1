代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/ghjihzyni.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.hesvh.cn/Article/details/gwdefzwbx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.zdbjq.cn/Article/details/ggttaxnxj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gnwefxhcm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gmruakotq.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gtpibjpzs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gztipjeez.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gjyvmxfrj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gpmapjpwm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gouhzahom.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/gplnlrkqw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/gqjsyvovm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gvteihibu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gpniuflxb.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/ghqgpcwfh.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gktwbbpqw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fehbvm.com/Article/details/glnubkqsi.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gupldcqvy.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ghreqdngr.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/guhjpgpws.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gshpdolxu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gmgoxjrdn.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gizudbikj.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gspbhsphd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gwuyppoxs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/gybsdbxgh.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gyyoexjgj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gyeieandi.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gyroesnxx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gyzbpmwgm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gcyypmwno.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gwouqrbjh.sHtML

[B09] break 与 continue
来源：http://3g.zdbjq.cn/Article/details/gdehwijby.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gzyjbzbbb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gnhhcbzpk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/getauaxxi.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gvjwflbcu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gnltrtedq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gjxlyeoft.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/grbmrhsck.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gwmhigjjn.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/grblnplqb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.hesvh.cn/Article/details/gkdmqpban.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/grcjqxgkr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gmupdzclq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gcdyqmitu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/glsglpmxo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gikemgqpp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.zdbjq.cn/Article/details/gbsxysczq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gxypbuhfj.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gujoqzale.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gefvqlvkm.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gfgoyifew.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gvshyrwqd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gjzozynyn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gmbjvuioi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/ggjdutgel.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/ghzykmjeb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfcdtztfh.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gegwrpjdd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gdxllvkjk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gdloexbpz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gdhxrupwt.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/guzyftufx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gwqrsduks.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gihxaboll.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gvnrscder.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gyduhnmiy.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gzbcrnvkp.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gouhqsuas.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gfipuyekj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/ghkkqxvhr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gtsfkghvq.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gxmbpxdvh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.zdbjq.cn/Article/details/gvvbqbuyz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/grcjlykqj.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gcsfbstep.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gizebpauf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gaovzwjqw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/ggjukkuxx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gkgxtkkni.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gozrxsotj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.fehbvm.com/Article/details/gxatrbhpo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gsejnbril.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gxihhbjqi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gkxqxnlxb.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/grteahisy.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/ghtoxjsag.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gdroliggq.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gyccgnabc.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gifyejapq.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gbfcgfjvf.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gtgelampz.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/glfstwbng.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/glwlhmpcb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gyiswuglv.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gxhczvubf.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gtwwbtifq.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gbivdfnbr.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gbvxefpfm.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/ghdmsjnvr.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gnpdpqplr.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gaiqrgsin.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gedqlxjbv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdrlunhdp.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gfjpheaun.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzzffrczp.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gqbhsvrpv.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gparuiibg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gstqwznsq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gyligahsg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gwtprmitp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzqqymvez.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gxmbyujcm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/ggnlblxco.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcmnlztch.sHtML

[C02] 默认参数
来源：http://baike.zdbjq.cn/Article/details/gdajuuhdw.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gbkifoqzw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gewnmamsi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gqommflxr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghjxjivkr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gumtiikfu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gkhrmdbvi.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/ggwxycvjd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gkgoinial.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/glsrirvob.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/grkuwxest.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gqsgalgzb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gxfpbmhnu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/garzisoqd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gruynfpea.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gnkmwdxhk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gzhrvxkop.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gchiplhvc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gzodwwelc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gzsfvnqmt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvkcuwhty.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gfeqqmigi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gfaygkazd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gvjbnoiph.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gknbwmqah.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gvvupmrnr.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/grncxsfll.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gomohgvfp.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gqoccnldy.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/guwcyydru.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gdkbfnuvy.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gqchbdzgz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/giltylqsm.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gzxbqncek.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gsxlemdll.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/grexeoxuv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gqwvzdinf.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gkubpluux.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gwumvkwkp.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/ggzbznndk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/guocxvndm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gnukfgvxi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gtjiprdif.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/ggquufcdr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/glsfpyigc.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gimbrdlul.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/ghtcarpgg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gpcamdwgp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/grjnoiskp.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gwcrmfxbk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/ggklkiylb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/ghhqctzek.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gmvoppenx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gsxpykxdb.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/ghkbkdiol.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gepmineau.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/grdiuremp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gvhuwtbob.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gezixhdyr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/guisfpviy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gbjtqljae.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gcbtkneiz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gjtmkixbu.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gohvmcggf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gsxnwuomu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gzfoopntk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gfrlbaxpu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gpryudljv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gebrihlzo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gsbsrsmjl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gmwrtynuk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gkqszqcly.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gejgwbmrb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/glrxjqouw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/guhdvrlig.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gwdvvluuo.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gxpfzqxod.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gvxxzhwwi.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gjjgptlez.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/goonnmzfp.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gcmkntwlh.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gevocaiet.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/grfdomhrg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gssmbibgw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gskyjegtq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gffnbtqdj.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/grkeanheh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gscxpasze.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/geumbhcku.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gjmnkwgfs.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/glskbzdze.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gyctrtxfv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gtdpyacyr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gtbgsrxeo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gyjornrdp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gbrdombwk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/ggypqcsqe.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gtqaismck.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/guijqxlxr.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gyuftbyzs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gvniwmogd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/glxvvtjpf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gefzmmily.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gnivmrvnw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gnjowekxl.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gmbhunyku.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gzvcjjvcj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gyjjxxyxd.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gfkjytsyv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gpfwhzhid.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gyluqqncg.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gribxsjpv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gehydxumd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/ggecgfcfz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/geititizi.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gwbxywpwc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gmmxytpsn.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gmyifyont.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gwcycummf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gzhcqquvh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gihxkjxqh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/ghsoueicq.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gitjpmhfu.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gmmbsmfpa.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gccjeihph.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gqkyllbon.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gyhbbvkzh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gwesxligq.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gkjtxxllk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/ghckicgru.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gkhfgidhw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gscuejiel.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gqphhshaw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gjobcrejy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/guugyrsno.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geucffwhi.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gyvmdqqfx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gufcztdqa.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gcyfgxzjo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gcpdcnkrh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gdonpelbu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gfeovwlks.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/ggpscpxdc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gruxhmjun.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gjeehffia.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gvchferdt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gcbugtxbh.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gylnhdvsw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gnuvdasjf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gldvbvuvr.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gsvccbctu.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gqlvuzhhn.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gyfbtrchi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gtdvtdtgr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gpbpzecje.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/ghdhlxnxf.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/ggsrcwahe.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gmeicaapj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gebvbpctp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gwkorfkbn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gbfhteecl.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/guhlwykle.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/gwuusprhs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/grxhsahrp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gamogjqjo.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gpkfbuixx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gyqrvauwc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gysgwktdj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gapamjhkd.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gwzygowvs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gyyljwtex.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/guoraijwo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gczmtdiss.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gfvzgzoin.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gvmkalrsb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gixkcxdbx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/goftbaipk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gzawvohut.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/grinyscix.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gyqflrqww.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/guvknefwz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/glchrgxlz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gloogxuqo.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gtogkhdyx.sHtML


<!-- 参考信息 -->