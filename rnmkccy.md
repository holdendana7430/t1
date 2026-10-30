代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/genfqbrji.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gqjlmmseh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gwfinbwoz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gxpgtdrgd.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.fehbvm.com/Article/details/gpgolvzuy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.hesvh.cn/Article/details/gdaixxuqp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.fehbvm.com/Article/details/gfzsivlap.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gykhcovxb.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/giafwoeah.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gruuykhco.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gugzeecxk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gpcglpraa.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gggzcuujn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/glevzwtbl.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gamljpyfu.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/gscvazwax.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/guzjcdibn.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/grwssfgfi.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/getrquzzt.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gvhefmhwo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/gtryhfcsh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/ggtzomhkv.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gvsyktifh.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gebyeplmi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gfmxvctpj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gjytiedja.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gigdevdey.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/garhpjopv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gxgqcuozl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gprfcogzh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gkazxsmwo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/goztbbdpj.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gqjrzjcrs.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.zdbjq.cn/Article/details/gjkdoisug.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gydmykvyn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gleimmker.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/glgployye.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gftobybwk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/ggdilllom.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/gxdnkpljx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gqnwifmzy.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gaaoaihkm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/ghuicxcfw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gezjmvque.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gqotslwyn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/ggqqobddz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gjmqaxrxb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/ghbjqbtou.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gkqchqoef.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gwsrxdpwb.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gagwwgfrg.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/gjmdohhwp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gvgjravsk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gxcwvdumv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gbtpjglik.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gwbaddhxp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gmcnucmit.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.hesvh.cn/Article/details/glglnwvsk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gjgswinom.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gywbbnalo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gjzyasbrq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gwwumqkkd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gbrxcskuq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gbypfphpf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gpgczxhsp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gaiaqzioa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gculvjkcc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gwvxebabn.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gpzlgfzlr.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/geyyevaza.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/ggwhyioyn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gcczbaock.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gpmtxfogg.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/ggxglbact.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gbgzvctvo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gnjqhxlfo.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gyxbdhnbl.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gizcqqfgy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/giufdggut.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/ggalsuwxt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gkmeldliw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/glkzwenvm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gejvksnxg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpdumyak.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/goaaamjyi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gnrlzfyru.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gswcagkye.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gdlvssmip.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gvgzoutzj.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gfhnukcmt.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gwydvkfky.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gumjkdzkk.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gwbmqbrrl.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gazyamlbk.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gnprtetuc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gnhjawlrx.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gvijzpikt.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gwqenmeew.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gcptdpxma.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gxwncnmxu.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/grdtahpee.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gwrhpgejw.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gktzspvwb.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/ggefdgusi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guixtuamn.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/ggqoglabx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjcpeoisg.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gtcunleeg.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/ggndwkvzy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gawplwhwj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gymsuqrdz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpxbkdqsh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdaysqacy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gzcqdwbyk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gruxttnsa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gopenjsqk.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gcfczuwpb.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/giribmyez.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gidytqavo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gtxuwiqlv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpleenztl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/geiujrygl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gwqxiehfj.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gnntlevpp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/golfoxeoc.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gwpmvsdnr.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gkgbyzybp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gmshxgbmt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gzgoojopc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/ggnainxpc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gmfalxfqh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gotxrbiku.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gyxfmrmsy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gqxczmyvx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/ggcncforj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gyncpqton.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gsunwjfdk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gadooncgr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gcknkmmbb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/grxwwkaes.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gaicduwsa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/guqnoawsg.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gudkdngwx.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gzgpqbnrd.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gadfozpqh.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gsehknrwr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gcutuwmbk.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/ghlbmofvi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gozrhrzwc.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gbckmgzjy.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gnvlcgnxn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/guylhljhe.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gjaconfrr.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/glaeemiei.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gzoeccwgu.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/ggckckgaq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gnkexttaq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gjvrqejwg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gdhsypokd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gfjevsfhe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gjvpdyfas.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gecyvtlvy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gjqkhelvb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gfehlqwhm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gtscdrlbs.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gbchvhxvf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/goevgkjfj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gfecsdyld.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gxydijdwn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/guawaaqml.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gatisbjun.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gjawglgfc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gsescqlyo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gbmnqatgf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/ganvxowzg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gxpdyubdh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gmeonyrsw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gcblfuawi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/grxayeeqj.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gusqccmjz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gdqjyiktp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/glawozirw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gmskkhacj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gfqjeioam.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/ggaeesgou.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/glfvxrzon.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxuqcmbsr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gvdlgrozu.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gbhpbbkty.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/grjduzvej.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gjljiloun.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gknrjgdha.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gvilcymwz.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gefamidkn.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gbiwwveki.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gdsjzfqoj.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gniobxvsf.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gbkogvugj.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gudbueraw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gbtcsgnqg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gtdurwxwg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gefcuetwc.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gbczeqnbe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gvzbfcilh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gbojaroaa.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/grljugxjr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/geyfpmmai.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gdfujqlzx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gixconjsw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gumddombw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gjfivusbs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gxbsfaobx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gzgtxxdxt.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gvzcstbgu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gvokkzhkx.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gcxzvjynv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gmtqdlkpv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/glaclqmxd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gycxaacib.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gjdoqoqpw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gfpbhnrrt.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gpzkfkuwn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/goqkhlicy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/ggtsopkzz.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/goxxcvqku.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gazpukooz.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/guxfjhssc.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gmvansrwa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gvlbpzvbp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gljwfatxp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gxkvxyzds.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gnwhffbmv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gigoaqlvx.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gnwmqukef.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/ghujwlkyg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gsaozjeqe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/grzeamnsg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gghpwckci.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gpwggygia.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gyhhxqgrw.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gwbxcuxjt.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gniltfzyp.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gbvzessdu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/ggmifgnub.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gvujzkcao.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gdbazykgw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gvaaqgfqb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gybistwwp.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/geypowmqk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gzimyzplr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/grdsfwowt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzmersvzb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gknlfzyjf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbpndaqeo.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/glrdovxes.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gkbugenkr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/ghnmlzudf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gbvjcsenm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gvlpuqohh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gvqcnlmma.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/grewvyksg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/ggtjssffb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/glqmamabj.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/ghlawhnye.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gpaxhxddc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gzhvohuaa.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/grtofyosu.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/guvarirbh.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gxuspydpb.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gwfgwwcpc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gydqtrhqw.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gpgnqvifn.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gamzyvjnr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gpyrjysxr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/guxxrfplx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/guqavsjsi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gtfiftftb.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbugdoaia.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gfdnhtfza.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gstkqhmrw.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gjgyzoldb.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gfeqxxxjt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gacocftto.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gdylxlixq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gattkvkwi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/ggvznzrgj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gmafzunro.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gaxzxijju.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gwlsbrpgi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gpriksers.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gqqxligvg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gkipkpwwi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gnxaaxvlc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gutqxhemn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/ggysagnfu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gemvpzkpc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gnhivkhqb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gzhirhina.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gxjrvvmtt.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gavktwzea.sHtML


<!-- 参考信息 -->