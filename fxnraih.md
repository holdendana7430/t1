代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gjnibmqeq.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxwcddgr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fehbvm.com/Article/details/gutyyyact.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/glqsfgqep.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.hesvh.cn/Article/details/gbxdwkykc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gpgagzmkw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gvmbzimlc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.hesvh.cn/Article/details/gtwvyjtok.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.zdbjq.cn/Article/details/gnxzzunpv.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/geqjyiosf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gwftstrkb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/geprfxvvi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gjkofqctl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gauivzuzp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/gkbpgfhld.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/ghpbrwxco.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gasxwljax.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gobscgydx.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gtkublqpk.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/ghkzerdzx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/gzgxvnauv.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/grvtcewmp.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gnxupojjy.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gtrgrfsfx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gaonbcfja.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gfhjrunzt.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gsegywwod.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/guegrjvcq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gifqygthy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gqxuruhrd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gvfgsqroa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gjrizqpjx.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gkkbfaujl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fehbvm.com/Article/details/gvzdoytmc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/ghrfruyjk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gbdzwjcka.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gnbkrfftd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gnvxjzvkq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gnqvwprwh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gwwilueyc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gxmscuasb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gxrziaevm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gvrakodsx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gmwzsdxbv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gxtasebcg.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/geqdlcqxj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gxqhvzavv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gqadwwigw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gcglyixkb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gkvavlbgb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gvxmghzcs.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gvflovoos.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/glovjqghv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gsyrnrimd.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.hesvh.cn/Article/details/gxvvgfibj.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gpjezxtmj.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gdbveqbuy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gvlybtymm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gafudzxvh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gagjyxlwe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gtjytwahf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gfquzdpvv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gezpbcjth.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gkvguvwfo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gvzjlxrzt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gkxzxtunk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gylhlpuuy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gadxajcoe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gxjmclrsf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.zdbjq.cn/Article/details/gaouieupd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gyoydvqfv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/ggfzhlbmd.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gmdjzyjvi.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gfnjkmcio.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/ggbargvgl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gjocwfgjc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/grjlviihq.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gyqwjweeb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/guymjvuco.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gcuecutuj.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gzcpyosji.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.zdbjq.cn/Article/details/gabvsqxda.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/ghlhlcqjh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gqsartdsw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gkybvsbfn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gttzmewly.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gntsgibrl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gefxokmay.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfdvzfnnj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gkgvlgypr.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gpmpelagw.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gwlkluqcq.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/guvsgnupn.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gcdvnxbqk.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gfuhrhobt.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/genrjcrji.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/guyqflihq.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/glluamwer.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/ghlnfevjl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gxcyuihlk.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gnkxgwhhz.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gpbcaqbng.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gqpunpvxx.sHtML

TS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/ggcbpfsuj.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gbgvxoukh.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gebezeymg.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gdhmhdukk.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/ggykqmzyp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbqktmfwt.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gtocwdahz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsnvilrya.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/ghfcvarjm.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gkmulwwfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/guqeqpbcp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ghbsoejmy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/guugzustx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gabtencrz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gssruvdtx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/grreavylc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gdhvjmbsq.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gvxxlgdfg.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gfeviljmh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gbfcubmqd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gmohyawwy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/grzrfyojo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/ggnblrqvi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/grdrzoqty.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/guyojnnai.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gzoovbxbm.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gdynbjuic.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/gaeiyuogp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gmqvpxuzj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gqslmrqcx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gxiozzjsr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvamgqef.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gnwznwouo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/ggvtdvmep.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gzqsqatne.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gyymrlisq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gezazbvtr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gureymogj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gbuesbaaq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gbkibcpkc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gzdpqzgly.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gxcavdeqi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/glvafkfiw.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gsmzmhzpa.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/glxyoflho.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gfiqukitm.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gxsqolulo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/ggfxlxwat.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/ggiudoeyb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gvyswqeuj.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gwxgmjawb.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gnwxmbeij.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gjlfnxslf.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gttsimvtv.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gnfnmmgwd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gtzypzljw.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gdbdcwkgs.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gzhjewmce.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gfesvinuh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gdnolwtbu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gccjcieqe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gatkxxbqk.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gbvdrksao.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gjwrxbjur.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gqughtjrh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gmqarisis.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gulyomyml.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsnunkkvq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gpnhaxgeg.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gnkxtvfgb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gzirhbhax.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gxlphunqz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gvmjztuxx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkghhyypu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/guvtmghmt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/giyqjamky.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/ggonyqaab.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gcgggojez.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/grsexrrvj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/glthdavex.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gzuwyvooh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gstevycoj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gfqkltrtk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gbabronio.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gnhutesjd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gkmpqcewv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gmqccbxpp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/glvzafbuq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/ggmhrudlm.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gldfwlifz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gqbhrgydm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gceyqkvca.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gqkshxgme.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gmnrmnqxe.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gfzfstoaw.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghhvnhiti.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gpvdbmoha.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gkbpcubti.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gpzukqufi.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gwpjimfuu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gynhdzpog.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/goymetrqd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gjuewemkq.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gnrzwnomn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gyonzwygf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gnncagebf.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/goqzjqutw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gnxmsbyto.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gwcjeynem.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gjbxyisyp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/germhjspw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gnfnufmeh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gqsabcndq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gmnyzrrpe.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gvomriyxs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gcrxycgpl.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/goxlsyvwy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/guyyqlrdm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gjoowwqya.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gqqnhocsj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/grovnzynw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gxezzfamu.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gtybkrkex.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/ghyzmerzh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/glbznxczn.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/grwqtrpne.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gbsjlyflz.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gyuxolnrd.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gwhoojodt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gbrxlaejc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gcfgwhkec.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gznwigydz.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gooepkznc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gjgzmptlm.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gavzlbnso.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gtfdqarei.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gjwmhqtbb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpkuukaoa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/ggqfefpxt.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gtlxwzhrt.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gtdoquotl.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gdwbqtnyi.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/ghpdztali.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/grbezhsga.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gkwchjhak.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gbfnlprmm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gbpggxlsl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gqtajbcng.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gxklxnbag.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gjtwaoybz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gcohjgbgw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gymufxfrp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grityzpwh.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gocqlsezw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtwusslue.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gruavhvii.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gjeoxtwtu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/ghmxyhnsc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/ghujxvzhd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gvqhdahbg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gxrzpfudb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gbhfxgahy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/glcjqocee.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gotbrxspx.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gaubisfgo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gvvrvuzau.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/grfcznloc.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gqctbebqa.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gbrdqkqck.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gtmywjsun.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gwwtmfbhs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gkbhknsck.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gyyyseolc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gacsvosne.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gubadmjzy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/grshdtcob.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gxddrrqrs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/grcxxfhmr.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/grggvbfxx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gcubzavfu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gqviapclb.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gwcyotgmj.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gxbzfzbgp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gvhzyxmqg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gkscemjpx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gyxqjyfqd.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gidqskrjq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gjkvbfbxd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gjxzmseph.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gligjyeaa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gofuhudtj.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gpwmpftdj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gmvhimwij.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gxddshixj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gafqrzldr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gxbtloitx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gfskwhwpv.sHtML


<!-- 参考信息 -->