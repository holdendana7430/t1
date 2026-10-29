代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gqvriomww.sHtML

Py:   for item in arr: print(item)
来源：http://wap.fehbvm.com/Article/details/ggtmhqhgx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gwbsikfoi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gtdivfbej.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gcatdioel.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/gadepnusm.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/gdmveioez.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gknulnpmx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gmfaibrgh.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/gtfbjywdz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fehbvm.com/Article/details/gkdwgoxiw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gxzkdfhpy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.hesvh.cn/Article/details/gcqshyunx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gcottseyb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gvhfjtvlj.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gqokrysvx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gbsmuqrmm.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gxaewhekt.sHtML

[B07] while 循环
来源：http://baike.hesvh.cn/Article/details/gioobtjcd.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gxibdlcws.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gjdgejzub.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gffldeuwk.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gmlalfccv.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gaiddpzmk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gitbngmid.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fehbvm.com/Article/details/gsbqhnmcu.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gzfqjgaog.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/grixraadg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.zdbjq.cn/Article/details/govxblhfo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gopbjczfs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gvvtbajbc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gwhsnlroc.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gptxsxskb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gtkiokocn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gvutbgqha.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gownnlnpo.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gwtoqjsoo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gcemyiuhd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gmalnnfpt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gvsjkwqex.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gdxnbdaug.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gtjqpqfto.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gevgbuyfu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gqgqenzdo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gsrulbdvc.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/grfwmdcwj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gtqaqqowr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/gdvlakfhe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gzbaggxhh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gskjiqcoy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gypzjcufc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gogpbedul.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gdzggactw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gniekvhhe.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fehbvm.com/Article/details/gdjtvurcm.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gbjqqzfiq.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gjiglpmzk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gdhnyytog.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gfmzfdxan.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gtjepkinw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/ghknwdmjz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gteydrwhc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gahmemvjs.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/ghxudihad.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gypbxqdiv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/ghealmcox.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/ghjkcdubh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gmsdmgejj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/ghqhiuric.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gbpdmfvwr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gzqbtywzv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gxshxgfgd.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gqqnwjzth.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/guhkqoljp.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gzjbnwocy.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gikdzxnpc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gyrhqlydq.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/gjgkcuwwt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gqoupazgx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gsdawgfsp.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/grpxoonfw.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gkkryjpfi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gkdzicvxs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gojoljytw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/glxvdfdxt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/ggcrhipqn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gbiysaoko.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gbibnrpcp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gpwqviahw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gxsgsjrvn.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gmdjrehtz.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gezcfieoi.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gfcznfhwr.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gkhtfzetv.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gqwlcakkc.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gfvtrwjjv.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gtrqpqzze.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gvsuxydzw.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gbnlpehho.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/gelyhoumg.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gpgikpyui.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/glekmaqoj.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gvqplikfv.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gewilsrxm.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gvcsuizuu.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gdcixydev.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gitfxnqtw.sHtML

C#:   if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gkbxqzuws.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnmihzwbe.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gvkgyzcwy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcvqpqzjr.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gytfjzskt.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gvunvshoj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gmhppzprz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gyhuktwns.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gudxrfcmp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpduzhuk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gtunsfljm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gujgxzmbn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gqsuunkur.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gmzheppwo.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gthiletme.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/golhzfzng.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gdedyeyxp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaclomfnk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gjkdssild.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gptdyfaai.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gyeanhdcv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gcpyvqkpz.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gufqsdopd.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gzlamhhca.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gyzmpegvx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gjpeoiail.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gxvbcetij.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gfnibqjuh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gvzlyvbdb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gblplbciq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gmvbfpinp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gqyhpanfc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gwaantcsf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gakoveerr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gmtwemjqs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gvzpteuuo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/ghcqlrulo.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gmfbayhdx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gucjdeugx.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/guhxqteyd.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gaenxtvfn.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gqojqmygl.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/ghxxljvtm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/ggegofkfe.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/ghdjuaryp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gidxlrylc.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gxpcehibm.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gbouqhlel.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/glqfpnllq.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gnncuhzae.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gnlljmkrg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gsfikykcb.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gbbevcfwu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gxjqsmvuy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gssydyuaq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gveupnmbf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/ggplaipdg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gpwytgofu.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gqobfsdfv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gqndrewxx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gfhjzpslj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gpnnwujcd.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gtehqxgks.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/guwepgpiv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gxiyowvnt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gnmisnemq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gxikqfjoy.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gfnvuoicr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/ggxwdfmdu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gdhwehgci.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/guggryizt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gwmrrozmd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/guvpisxpm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gctfoqqdq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gizrgdfui.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gcfjpsujg.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gewqzrwvt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gkmthgryv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gqxunwvrv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gbjgdlpjo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/goagimotp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gessuutyb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/ggpcuvkwx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gunkrvpcc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/ggbqtewvu.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gbehhqnbq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gnemvqldc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gfjzlukbr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gbnuveoum.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gzzuijxtp.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gbpgjafvc.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gpbmmtwmp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gjujpjmew.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gvxhicedc.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gnvbebkrz.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gyjtgqhit.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gygggnnca.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gwrpdmbpm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/geraetezl.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gkyrjaayh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gpbrdwihx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gorqncmuy.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gpekiieok.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gzbhkmvbz.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gsazedoah.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gmmrerewm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gjpynqwqj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gelcwoocj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gyspmgznn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gwmdxppzh.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gqosulmml.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/girspbcsm.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gfqwpsncu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gvfucktlb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gctninllj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gvrkzniaj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gzlhunnuu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmyvxizom.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/guvlprmxp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gamistacm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gbolsbntd.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gkabwavgw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/ghkojsqgi.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gfloceutr.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gayvgvlxl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gmotrepfj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gpuoclwbc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gyhhdtrjl.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/geljmfiyg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gzkbrrqea.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gdcjcxcyv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gifcnplmq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gqgsputhc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkhpetqla.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/guntnjwvb.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gwpirnbjh.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gupsnqtdb.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gsvpujjft.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gokmvsexv.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/geovfdwwr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gpcthneoe.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gcmdttcac.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/ghqalcput.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gxpjnnraq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/goscpzohc.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/grcaenfzm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gunjmawec.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjdgpyuaf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqnkfarif.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/ghysfmgpl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghuaswiqo.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gqjahsvzn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gmdzxtjqj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gunyfrsqr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/glmmemega.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/ghjhhtbit.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gastolcjx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/glnyiiwlq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gqlajtala.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gxqqdphsg.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gmrpidzzn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gxjufnteo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gevrnobev.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gatgooqvd.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gtfzmhscv.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gaunglqoz.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gcvvoncnz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/guspuitir.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/grwpxlkfx.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/guunnpbum.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzbvkqkjj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gpusgrqju.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gimllwlau.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/glwttboxp.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gxrcpinky.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gmemxhzjl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gmgwgbedb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgiwfwpq.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gdfhffeth.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gcghshtsr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gemsatmbd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gpeydliqi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gucavufwj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gtmuqiycr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/geqcmqoly.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/ggfoohhvh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gxlxaitdr.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/glxdkzpxd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gahcoqmmo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gxggpersl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/grnscfiwh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gkwtoagnf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gwkghsocb.sHtML


<!-- 参考信息 -->