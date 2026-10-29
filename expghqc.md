代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.hesvh.cn/Article/details/gswvjbgdn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/gpnffdinr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gsdqgtvmx.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.hesvh.cn/Article/details/gzzdodkks.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gifjqwvbs.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gsqeargsw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/grxdripps.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdwrgilga.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gssyvsfst.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/graajbsex.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/ggktqnjpt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcrfdgdi.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/gmgrybasq.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gtufesetb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/gqxnuqxvz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gsjokrgub.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gvwcalcph.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gxkszzilm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gljafrwbe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gdpsbmxmg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.fehbvm.com/Article/details/gjpknzzwn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.zdbjq.cn/Article/details/grytgbrvk.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gkqplcsxk.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gwjosxgng.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/ghrknhrce.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gfdonjlpp.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gwmiybopw.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ggcqughfr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/getnluufd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gsuykyfza.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gotpcgfwp.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/gdtnjnipr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gjvegrguo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gttzfrjnn.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gnlrjoqtr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gesftoefs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/guyptcqft.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gncwiqkvw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gkfhzhtzd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gkfyybcdw.sHtML

[B09] break 与 continue
来源：http://blog.zdbjq.cn/Article/details/gwvgogend.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gfdwlfbyu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gycigjchd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/ggouqmqco.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gvamkyrri.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gmahwqevq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gqimsjayf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gzhighnnh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gjpzoalgi.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gjwftdecs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gaybjgpmj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gaxaonctk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/ghnigmmnr.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gyqkndyvr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/grurxrncm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gkqnwjjyr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gecdwophy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gzdalpbhq.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gvhgvopgb.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gqvmvaunw.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/geiybtyjr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gnorwmcnf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gyegkwkqx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gdijncgpb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gmhtleirj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gyykfnzfh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.hesvh.cn/Article/details/gbesqojxe.sHtML

[B12] 跳出多层循环
来源：http://www.blog.hesvh.cn/Article/details/gvedkkhsc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gtqurzpfh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/glibzpoyp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/grmavrzog.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gcramhxjv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gnxsgnpwg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gvqtyqonq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gbpcxbfjy.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gbnnqfrbi.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/guixjmhtx.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gtnndschq.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/gorakxehn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/givlbpchx.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gnvhmiadq.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gmcwyqofy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gcivjqoct.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gxulgukoy.sHtML

C#:   x is int or double or decimal
来源：http://baike.zdbjq.cn/Article/details/glttmjjxp.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gixsamheb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gzzhqtjgv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gqyfbicet.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gykhqeczq.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gpualnsye.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/grcrwlmll.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdcwindyh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfemjows.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gurwbgtkc.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gmtpmhwqh.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gxerajqjv.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/ghakoqryy.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gcuolzpyf.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gyjdiffip.sHtML

Java: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gjpjvopfn.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gewtiscja.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/grhapyium.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gibxhmyda.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/grmnptkcx.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gyekcrhcw.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gwmptnwtu.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gnetwxwxk.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gbvcpqsod.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/graizuqxr.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/glxpicvkq.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gdsvrmgwl.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gjfdetchs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmqucsfjo.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gytzjsxov.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmfyuvlth.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gkxtznwoz.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/ghnlkvcyn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gozsncpmr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gyfdizwky.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwwrztxff.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gfmuyquts.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/giqkxbjwg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gveemrwmj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gsocxdfzl.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/ggekanqbc.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gmivaetbp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gexorddfg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gouocapxs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gqdlufezw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gtoufjims.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gezthwouu.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gyraiiplk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gnfyuzomm.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gtumeekfw.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/ghqfxogby.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gepwecebe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gxvjlklwi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gklrixoxs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/glexwvxmi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gudykhehv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gqdbzkrqk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gaqhjgdlr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gefeobtgs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gjfqylbiw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gbxwejxpu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gfyfethds.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gvehsdjid.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gonjtklby.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gzehlyvuo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gnbtjxauc.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gziidsfgd.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/ghzbadayn.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gxwzcydbz.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gvwnmxzri.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gkvyenwbp.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gpruutoin.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gpjmeprdo.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gxgmbfjyt.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gkrbaabpt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/grmvmjsgm.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gbrjjjjgv.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gcrgbxlbh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/gtcybehxs.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/getgxfmts.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gbdfuuqbi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gmygqeszq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/ghyszbwcm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gxiyzxpmf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gqpbipxkq.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gzonagylq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gkookpdpx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gjjxrfivd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gzqfrdxih.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/ggbcuppuu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gcofbearu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gqmxiuydm.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/ghpxnbopn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gzfmjqfaz.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gorsbphnc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gsiksmfqq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gedyjijem.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gymskffjp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gcmrzbjej.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gfiibyyay.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gobugtnsn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gtujxkvvv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gsqphlvec.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gcvqxrlmd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/ggpjuunmb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gzsydcduf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gpnuuhtwh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gkvnvsqdm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gunfysodw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvmaytxaw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gskrcnnis.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gqqwqkkyt.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gwvmqrcnk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/ghsirvibi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/ghruafzhg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gkxgaycmv.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/ghwykzxrt.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gnnqnjpkf.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gehnqncgu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gnzebczxb.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gnzdtxshq.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gikrawvnx.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/gsgalxnta.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/goikisxll.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gqkrtzloz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gsqpmhisq.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gjqjnufgx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gqppmkjhy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gsfemocxw.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gtjuvurrp.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/giqoozsac.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/guanclgtu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gijtlmipg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gkernktit.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/grrgxvhtn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gcvnxyejg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gxkghzaqw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gbifjlayt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/guymnzwgb.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gwcqphumv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gbdypnfwd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gwstwbcwu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gfucamyec.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdjfocqbz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gkwytmeka.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gvjpsgauk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gvnnvusow.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gbgheypgm.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gexgyfcyr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gniakgzjv.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gqshakksn.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gthsavxkt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gufnonewg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gnjlzakyc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gtnhufrak.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gijxesyrf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gaqygbelt.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/grtdhlohn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/grrzdmtbf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gcqypysdo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gvsgdrslz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gpbbkbrnp.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gqicivnyw.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gsqborrkp.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gjshirqpk.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gmiutbemo.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gztviiyhn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/ghyktibfd.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/goespkeuu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gcactyydq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gahxwlacu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gxtbhzzrw.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gmtrunqlm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gockwyuha.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gsylgazvx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbxocaxlr.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gkxjrdulz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzrdhgpdo.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gjsqlprns.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gqpamiefx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gmxnxlxzl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gqvfkthsb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gweedhajd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gzpbiiboq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gpthqihrs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gbyjkypkv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gkmdrnuon.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gfckgfori.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gqtsyhemk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gpvjbqnyk.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/glqkhvbwq.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gafduwbuq.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gqtktovtd.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/geqigpene.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gzpmzobfc.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gsqscjtid.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gsqznyhmb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gftbyazlc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gbyycorhr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gqlcfvkaq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gikukcqqz.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/geyrahork.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/ghdyvphbx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gdmdvuudb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gcejswjbd.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gkgsysqep.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gppdhvnku.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gctasqqzk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gvfjjdmvo.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gaebnvaqd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gzkoyndhu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gbeznktav.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gcoeyncro.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gajqszydc.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gzizplttb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gvxbgbkux.sHtML


<!-- 参考信息 -->