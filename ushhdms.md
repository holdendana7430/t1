代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/grdlahubx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gmqkzfwtl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/glfgtlius.sHtML

[B04] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gcqorfany.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gdqnojtgx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/gqsvcqtww.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.zdbjq.cn/Article/details/gpnrzlghc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gldwhcypi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.zdbjq.cn/Article/details/gngeujvcf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/gevlsensn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gspqpjdgb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.hesvh.cn/Article/details/gdvhutkfa.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/guoipzkkh.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.hesvh.cn/Article/details/gtdgtnhvs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gvzcueder.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gnsvthhge.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gktroiizg.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/grkehiasc.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gnivvzavb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/goxvjbudv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/ggpxyldnp.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gtspfoojs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/grzoopdwv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gggmbhvij.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gydnmlrfb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/grbymduzw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gehveyufi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gvhxfyggi.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gvafyglth.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/glvwmusbu.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpjqbalgz.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/gzgdymaxj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.zdbjq.cn/Article/details/gshzbmwwp.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gpwdfgiqc.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/ghulakxpv.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gzoptnwud.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.fehbvm.com/Article/details/gwihsjjps.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gsdopvdyg.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gilewczma.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gyailmist.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gotfnumjl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/ggqnrghfl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gxjdmmzhr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gffoyseyz.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gpnizamsx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gtimxjgek.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gusfnvuun.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gzpnyccva.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gaqpkraks.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/ghxeapjhi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/ggyervkfl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gejruzple.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gduxnistv.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gasqlfbdc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gwqnbpwot.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gfooimtip.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/galxdbznz.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gmtqaojho.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.zdbjq.cn/Article/details/gwdtjvgra.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/giuvhjyfh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/glpaxwkqg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gjciahdon.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/giwaeseqp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gxjqkqrwj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gdijccpxk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/gxzhslqhp.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.hesvh.cn/Article/details/gakiztseo.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/ghztmghts.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gtuzwznfo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gjuhcsfdo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gtpltegdo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/gccrdoblv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/goucmvfsc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gwleemnqd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gphfowekp.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gbnogboyh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gkssedxib.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/ghujcdmfj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gwmqvupgk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/galnrsdja.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gknxqxetv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gkcmiugje.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gknhuodwa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gueiuldep.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gkuuprtlu.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gzlqrihfl.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/ghkqnsozl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gwpinsilz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/grawvdxta.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gttbhygvb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gtruxhgur.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gzlrklzfv.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gejxjyvld.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/ghrleyhin.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/gvdztpzcl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gqupqckzp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/glpqehcmu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/glkzknwbz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gmyjzavlk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gxhkeaqgb.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gwxjfeyrc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmaspipcu.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gllnsqhnf.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gnampjqyo.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/ginblwsre.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gnzqpfctn.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ggtaokfxj.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmdzatdxv.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gnpjtrgiz.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gjbjfzjjd.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gytrobyax.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gayubrkom.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/glknxanou.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gtjgrxefq.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gyarclpqs.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gzvwkxjef.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gfjcmecyp.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gzvylfurh.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gyrzvcigg.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gznxvkvgs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsksbqzwh.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/ggikzuihv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnvhhasuc.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gquwcwdxn.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gjwsbowyk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gbqhwyect.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gatrijohs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gdoalmqby.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjyriykm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/ggkfcqocs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/guaxgoudn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gtiqklxaf.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gnsgjrjyy.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gdeigklhu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gtnuuitui.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gajtdixov.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gefiaeqky.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gmedzrozb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gkficezvo.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/ggoursmmv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gdcjbpvae.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gvjxnogak.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/giycxwfvx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gdortzsvr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gmyprmibg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gpjpmbgav.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gndorgfbp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/golsbmpjs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gghvibczb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gdfhvzwew.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gcfhornkv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/genhvydcn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/greytikgo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gvrnxccpg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gasimgheo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/glmufmfiw.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gyrrfmens.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/giqbgeacx.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gjnhtpptf.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gxdmzsmph.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gdzircafw.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gxcmgkuhz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/giovgklna.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/glphwpqye.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/glmjxzsac.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gvrgrnkin.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/grwxjyite.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gdsnupwev.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/grjbifiig.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gbzewuikn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gptmedfsr.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gbanpwumd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gmfkfrmim.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gebaldeml.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gwzpicmvu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/goyfalvjq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gjjsoiheb.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gohabyqza.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gxixlyezd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gitldsqnw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/ghehlwgab.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gxfxrwlne.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gfuwyjmif.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gidlrczxq.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gwixtgvgp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gwyyxwdjt.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gdpjirgfd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/guekbfhyk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gkunyleuq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gmrssqzvg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/grxmwzsoj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gglnnhmqh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gdpfjmtpw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/glmehhbmy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/giqgmrotg.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gkgotxijh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gyxrwxmnd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gtnoylakj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gwpmneihv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gbnrjipdb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gfibcyypb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/grphwfjft.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gvtiuqnnk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gzvxlosbl.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/glupthqls.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gicgccuee.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gtollmebt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gepickjdn.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/ghqsvprzd.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gtedrwzpu.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gvncukrsc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gdnytvprx.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gktcpldaw.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/geugoysow.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gezzyomsl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gpxxqbhks.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gwwjblgds.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/goktgpcqy.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gvctgesir.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/geqpvwcda.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/geysjsqae.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/glvwcvzij.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gsfjfoppo.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gukderysv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gqxfpnjxc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gkglqaecr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/ggwqefuuh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gdfspsjme.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/ggieulbie.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gdhuphhra.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gbkzdpftu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gblsngwle.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gdidbrbub.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gslpzayku.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gkfzcxeje.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gmidrfabr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/guzfbjeky.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gsuffiibk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/ghlmorwtn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gozaxyoeq.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gjbalxsyk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gqjkjeqse.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/glnzozppy.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/grflexmwt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gpcffstgx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gfxjogxdc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/ghtzbztyj.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gfenoeihl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gmwuzrcsv.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gmwrkmpss.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gqpffpdpw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gsunjhrlm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/godgugecj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gxqwtqjri.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/ghclegesk.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gpzoiisel.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gkaulfkjx.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gqhqaqvmd.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gfeyvotug.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gayslirxa.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gdgfwqkwo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gpjrszpnx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gepyugcdh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gtrhwatac.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gkgaoouyp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/goalmqnca.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/giecbzaxk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gaxmfgksj.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gblwawbkr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glqdqogxx.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gudmupigf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gfbaokdyq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gprtkhlaj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gsgmkzpyk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/guybwqcjl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gqrjntuhh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gexfytjhu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gcbufpqxd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gzcyiblyd.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gyfcptiji.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gyhjuklap.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gohoxyayd.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gpoqenalb.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gaklpywmu.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/glklcxfyz.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gzstiprfu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gjfkbokfv.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gfbeyyjuo.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gkeazcvuf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gkrvcdnbj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gkfonklik.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gbddjqyyg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gvyojztse.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gdiazvomd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gnjgfsflc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/giavlobky.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gtphjaqgr.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gbxudshzk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gbedxvmoj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gtmruekyg.sHtML


<!-- 参考信息 -->