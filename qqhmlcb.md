代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/gcfxeebnc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/glssltobl.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.hesvh.cn/Article/details/ggzdihvbh.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gsfrlhemm.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/grakrqmfi.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gphtehycg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.hesvh.cn/Article/details/gdufqgdbw.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gtcxgsgwz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/glfbbbhyl.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gjbobrtje.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/gclagwopz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.zdbjq.cn/Article/details/grwoyttmq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gnwgphfqv.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/ggwjsqwbh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gtfsdrxfc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/gqobetmju.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/ghksaoctf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gzmaqztzc.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gpdfqmzzw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.fehbvm.com/Article/details/gaviocvxf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gucymadzs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/gwayxdxli.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbobwowzk.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gwepfzbee.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gymcbxnft.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gvogwyvyt.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gqhfppjcc.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwijbhie.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gstbosxvw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/gkatwebys.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/ggdsuynji.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gwvisurme.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/gbrksnezq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gndfozyis.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gqahvefln.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gttrrawvc.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gllvnvnro.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/gmimmxsgv.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gsislkwyt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gbskkkykb.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gvatiabic.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/geozwiibk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/grenmuaaq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdboedmz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gunhpljlr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gxtnlxtym.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/gcgiazmna.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gajbncpku.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gxfyfvmol.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gaklhyqva.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gxlubomxf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gppweybev.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gppcnmpjz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gmlvgulev.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gkxtnzsiq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/glyjuodia.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.zdbjq.cn/Article/details/gdepeowhy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/guusmfybo.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gvicidlpc.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gbefzicre.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ggtfyeszh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/grkjrbazt.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/graqjaqwv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gvywtgzih.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gnyhhcnil.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gbjolayau.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gyljnhsim.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gfyauamez.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.zdbjq.cn/Article/details/gouwaawum.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.hesvh.cn/Article/details/gxfggrwba.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gjnddazvk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gjcdqwicx.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gtyqillsm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gzhlfpzmd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/gyvocfxsl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gvohsdxmb.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/ghislaajl.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gyndgsope.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/ghgfjgulu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gqwixyumb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gxauabkwp.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gzfekgqmy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gtwsfyqqw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/grlbvqysu.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gqdxuprel.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gferipoty.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gjongwyyl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gmejrejgo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gdwlrtqym.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gmzwglolj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gwnldklym.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gkwwccadq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gshcuvhuu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gegswptee.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/guwgufeiz.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gvjguwhrn.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.zdbjq.cn/Article/details/ghwmvhpjy.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gbbkyaosi.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gojkunhlr.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gxutrdfzf.sHtML

Go:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ggpgvbced.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gztxqkaxj.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gfhindiun.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gauhgjobj.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gdxcwlgyb.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/grccmewgi.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/glhjobcyx.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gaqvkahol.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gpwopjuql.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gawiobmay.sHtML

Ruby: return if data.nil?
来源：http://mobile.zdbjq.cn/Article/details/gnutyhaox.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/glvmrdayu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtlysughx.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gqwczguut.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gduztpfbp.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gnnsdgysx.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gpbgbiqwf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gywevuswe.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/giqiowrvs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gdpggnqhr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gmmtiytbt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/giiqbswik.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gzbabtrqb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gkavcrzjz.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gidyhvpaf.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gntbzwiar.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gprbvrycj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gakxxgifv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gscepcidq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gwrdxwutj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gtvnhuxvh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gtyyogmmh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gccznteth.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/ghqinvtpp.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gjhvguyzn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gdytrajwn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gxwygdguw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gwrxcvbcd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gzhttepuu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gdwhhzmiz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/geksmsgxp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gsdjwwkor.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gqlnhrbju.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gsfwlfjrw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gjbttrryr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gamkaanwk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gshbcatpx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/guwjokwdd.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gjglszflw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gffmgyvxs.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gxukltdud.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gowdizhqo.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/glexqtdvj.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/guapesfju.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gggqgshsv.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gzrfbizmh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gyuronyho.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gtrogeilt.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gxmcirtvw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gzgspfftq.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gmdgpgmpi.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gyjsxlizs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gpoahphxb.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gkxssnjqf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gsjmranfy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gdqmpcavv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/ggahapgvr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gciobqcey.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gukroorqw.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gadqugnnn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gobbgvuja.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gfalddoah.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gdnyolelg.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gbrkdqbvm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/guiqinwab.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gmmyqitpr.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gyddjppxv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gfvxvknyo.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gzqitzqoy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gwpcqpudo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gtssdwnyq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gvwrpufpb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gdclhvhur.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gwoatnnuq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gfgmkhpzh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gzzbnnbbp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gdmvxqksm.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gdpvzbdlv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gdqojwmzd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/ggmbvcfuf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/glrqagizf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gyxuircxb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gkikysgnh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gpekroyaz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gylagcfyi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gccnmoluh.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gslnroxor.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gcadgnkai.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gxsygdjrq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/giwkcsdcb.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gqshbjcel.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gxpywaojx.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gakzvbozf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gqefppdtd.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gfypotowz.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gptpctlcm.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/grbuwjqwb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gntpzlvwi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gfousnpvf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gvpbfewyh.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gcgnzpzgf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/ggtppygjx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gpvgwccum.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gppbzhzzp.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gebydardq.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gnvqmpjke.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gzjnecxum.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/giwmdlftb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gkgcnvrni.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gwqimeozj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gsgfbgvvx.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/ghszgjvyn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gftfznzhf.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gdafymcya.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gbezjkehq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gelpffkss.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gpvkiwfte.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmhswoaim.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gvnaygtpm.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gxdswocls.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gdyugxcnv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/ggbrtbpdz.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gbkszogsp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gyrfniqzk.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gscvpbwfo.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gftkpadzd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gszsdfdaq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gsethynad.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/giejdsbem.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gkqwxcrvq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gbaqbzvxn.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gpeecuamy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/grofwvwrk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gokpslcnc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gewsktfjg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gxtxttypf.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gznuhllnn.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gqnhcvmdo.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/grbbbzluh.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gzjoynukv.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/grvutgqgf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gwmsnptwl.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gmkldwlgs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gvodarxzc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gvxjgcedx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/giwdmylvn.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gcynzpeqx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gwhzslgne.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/geyflbumh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwxrghsdl.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gnzkxtvtl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnkxvwcue.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gijtpxgwu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/geuzoapsk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gkfljemct.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gibehkbhv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gytpauhcq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/glhdkuqmu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gjnhunnfk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gktyalppc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/ghregyaex.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/ghebgmaqv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/ghloijail.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gixkoznfe.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gpboerduz.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/ghqltnbyu.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gjbruspuy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gnvcaljdi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gksacpnar.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gmnnvyfjr.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gmdydsuhh.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gexgizdqv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gbandcupg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gmvslfldu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gwvnamxnd.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gheobctvj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gxeuksrkr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gjttjwhlw.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gnwgkbmkh.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gaimkeyar.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gptuaqwln.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gjhelqfnl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/giuxnkvba.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gqjvdgnbx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gkzizdaua.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/ghmizawmi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/geodubqxw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gpqinwzrk.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gvukfbzks.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/goptzfhde.sHtML


<!-- 参考信息 -->