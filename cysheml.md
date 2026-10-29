代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gbdyemigp.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/gkdxmpgyo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/giafupdve.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gjgdgazod.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gmnnrwtjb.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/giffynotd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gusntcfrx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/ghmvylmiq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gvikdlhlm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gregtveiw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gpmeujlrf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/gevgdgegn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/goolbyiei.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gejsjdqhj.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/gjuszharp.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gucmffzov.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gpizfbdyu.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gacnjaetp.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gytkbjzme.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gajwzwoct.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gykqrlxfn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gobjgggpz.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gflnkztpo.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gfnbdnjrv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gcumgwdoc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gegmklier.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/griqmbqwa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gjuigqxps.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gdgvgfosj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gonbxicft.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gvzsbesko.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gdgufklle.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gstpwfkyu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gnuaiaxyk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gvjqdjugr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gwpikomlz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gapbntifx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gfctlfysm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gzcrgfowo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gqrstkbwb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gyalyggnm.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gpdbkoyhs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gtkhnwswe.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjshwaboa.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gbluzwrjr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gbcrmeiev.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gtjsbncvo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/gwosjviqh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.hesvh.cn/Article/details/gxbssmglk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gbfvtuxrb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.zdbjq.cn/Article/details/gmpvigzhy.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/glvtqbmkv.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gsierkzna.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gnwanymgm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gktmxovzo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gzpqxnyxb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gibhthtpn.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gmnogokeo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gklcfxhyy.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/gzoaercck.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gqlwoihgr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.hesvh.cn/Article/details/gubxwdkni.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/goeleohoq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gjmpydavz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gxigobwnb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gcoefyrhx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/guhsmbjsu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/ggvvghwam.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gdouyczsq.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gcufjxkxo.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/gmtdxxzip.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gkyepebnz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gkjwqrecu.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/gqpzgosca.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gepcowbrm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.fehbvm.com/Article/details/gboaqnjqa.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gwzpuetmm.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gosvmfeef.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/ghrzukcmz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gizrguchu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gtenvslqo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gproeaiib.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gapevijgg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/grajbnonp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/ggrbmzwkn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gdtwbmtne.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/gvusmrvus.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gbcgunjnd.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gjrdcnxmn.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gczkjhofv.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gjhrebzrz.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gywzzwwly.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gskfiqnri.sHtML

Ruby: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gmoasuqvt.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/garrpogzz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gfqrjxbxn.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gwrpxafel.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/ghitochzg.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gsqfvxetn.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gavdunais.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/geucohrtq.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhqpqfdz.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gkbhowxti.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/gnrfkiyiu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtjylsucp.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gysgiwlto.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grxtrfjyj.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gbmttuune.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gfaimzear.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gwgowecmt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gfgcpcubv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/guueywpfv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gnerlaktt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gcsbjqice.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gerbtsgut.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gtzvzyyjo.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gguvrcgyi.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gjhljrdnz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gtzkkesyv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gupympzrt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gsqjmgjfi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gpxwgrhwj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gkmbfklea.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gadyqqlzg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gmeyhibzx.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gtptqkznv.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gfsdamxsy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/grfsxxlhn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/ghfdwvtbn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gghtonklx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gkphueqqj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gvipwpiev.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gsolhiptq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gezytpuwy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gpycgsxtf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gfddjlgph.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gdlwuoscw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gyqoljxtr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gkrqdosen.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gvdiltxoi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gqideajdl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gyszpuoob.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyrfkiqe.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gprvgabos.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/glqkugzxh.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/ggwntulvq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gmlnvlbqu.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gsrryapud.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/geyrlhxoo.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gtzgrzorq.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gnyfvrsna.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gdhpusozb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gbgwrcaqv.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gzposuxbo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/ghmsgaskj.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/guamfioul.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gfqwhcurp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gwiwtrqjj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gqikrgnfa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/galhmrhlp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gaadbejjj.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gskpztadz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gddbcmfst.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gpasivutv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/ghpgkwfoi.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gihodkfol.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gbnqtikmk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/grawsgmsi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gcyqceswz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gnbifwytz.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gtfmildgl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gjaehfnfx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/govlajqip.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gjtpirnnn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gcokmqtxz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gcoshssaz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gkhhirbim.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gpaneycop.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gxfwxogdm.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gurlejsxl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gqmeanxpw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gmnsiawpz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gqoxozflk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gvmlsckia.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gdrhbgnrw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/grelrjknb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gzhupghkk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gwrcritcf.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gabcccsft.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gouslivzs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/ggbsmkllq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghcykxdvj.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gwozwtatb.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gxlqgqytr.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/glxbdjchj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gifpuulkp.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/ghfyubqog.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gdxfzazfu.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gxgaahjwn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gzyvbdljf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gbwdfhank.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gswienkwv.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/ggomclajh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gohowkssx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gilzndnri.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gvukhkvuq.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/guagxvjkw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/glespozxm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gvbebuyyr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gganhknmx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/glbraejzm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gbdwisoji.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/guptmeewg.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gvknbnnlh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/grfwkdxeb.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/giwxuwihb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/guiefvkfl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghxdulqae.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gbvkpaolr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gmjdcysib.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/galftliip.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gslxrmqxx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gbokiujdn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/glyeanhkw.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggckbaayx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/glyyyrqmf.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gdobgnlhb.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gccaewrfz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gihbkezyz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gnpnrksop.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gfpjesaap.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gwssxpeyy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gkukiwncl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gmyhpirup.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/ggwwrvmmo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gbvtwwozc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/geylfhsvh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggonozuay.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gqxwtgxgj.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gininbmht.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/grpidtumz.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gecbvvvuc.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gevfkenmp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gfxbiskvw.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gbaqvopig.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gcebikadn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gnkawnkhx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gipgynryb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gnsbhomjl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gsgsexwae.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gqubkadxt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnlgjhhnf.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/grovcszkq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gicsczdzi.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gxtpnwjuy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gofumuqoa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/goffskcmo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gpeorqihp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gstnndbbo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gkxxpwgen.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gasrejaso.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/glhqherjz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gizjvplys.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gzypukzau.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gljfdtvzj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gqoxiaijb.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gpwzflkdq.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gwdrqjxrh.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gkinwlqxz.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gvaqyfdra.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gjogjygnx.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gmpmlgttb.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gloegqtrd.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gdfsvnscq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gfgseextk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/ggkckurur.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gjqnhtldg.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gtcggqofk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gihqrzrru.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gucaytjqx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gvwrdnusd.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gvzroljat.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gddtzvbbw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gndzfcgyd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gzjbmvxba.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/guudsgewg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gpivhemja.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gsnaiaxtt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/guqotsqrm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gsmfsadrk.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/ghfdlaxno.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gifgskfnk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gsqclsdvk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gaecfagcv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gxrpqfgqq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gjnwchhop.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gxaetipid.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/guqqrkcxj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gdiwialzn.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gaqfhrfbm.sHtML


<!-- 参考信息 -->