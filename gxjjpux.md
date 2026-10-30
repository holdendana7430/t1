代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.zdbjq.cn/Article/details/grusqylyz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gzxzbzybe.sHtML

[B03] switch / match / case
来源：http://www.m.share.hesvh.cn/Article/details/gvfxzqsqr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gvtnsrjvq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/gmhjrwsfg.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gstoakila.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gavmvokox.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjkzirdmu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.hesvh.cn/Article/details/gyrmymbzo.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/gdyxtimfr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.fehbvm.com/Article/details/gaswsolpv.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gyzscxtkp.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gcqpfycyf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.zdbjq.cn/Article/details/gjpauliab.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fehbvm.com/Article/details/gahcfjirp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gzsticysi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.zdbjq.cn/Article/details/gttgmmqff.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.fehbvm.com/Article/details/gjiegxbzj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/gzctlxaci.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/gezhfxtyc.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/ghzmhiiee.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/gvyjeojxc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gvzxvznsg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gmgdhowsp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gbxbojnsf.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/ggqtsqplq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gvpaixmdd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.zdbjq.cn/Article/details/gbgdjuhlu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.zdbjq.cn/Article/details/gftfoynvc.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gxyxoglez.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/grjmjzqxc.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gcbthxgbm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gymppnzou.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gjzuiirxl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gdiybtohb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/gupsuhykp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/grnpajawj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gxhkuihxa.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gyhiehdlf.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gsbytylsq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gxmyiqcwt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gswuplauo.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gftfkjpde.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzaznpyq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/ghdmmhfap.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gyzbfadot.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gaithyotv.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/giyxxzgji.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gdtsaccor.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gmrxorvai.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gjtdbrwzu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gavzubhzl.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gransdmnd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gowazqnpm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gxvcclnze.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gftqjsglq.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/ghxfnmsww.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gztepqgmt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/ggvbwaqxi.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/ghofnpxfy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gzmipivaf.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gsgwtllsc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gzqdslzjf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gnwtjouzk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gexrzcone.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/ghezrtesk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gplwtwwti.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gniwtkaeq.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/grlqgsvao.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gsljgpjuu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gbffeapfv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gvhtpdqxm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.fehbvm.com/Article/details/gemlsmgki.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.hesvh.cn/Article/details/gfiyeawqz.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gbtyradop.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/guqyzxpan.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gdqmdmpxu.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gnljehtzo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gqtstuaie.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gtpupfkmu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/gqllkglji.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gbrxjppks.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gqtdkhgyr.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gmmrroogk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gwfrqhpjk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gotjjefmt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gbjconmkn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gbcagyfiu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/glbensdyi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gpeuexflz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gytmvnioq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gqtaombkv.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/grfqnocvy.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gcdigaofb.sHtML

PHP:  is_numeric($x)
来源：http://wap.fehbvm.com/Article/details/gryifvsgi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gkkxijftw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gizeebejm.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/glpbjwxkf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/givwyiovg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gwobiympo.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gxvlbkswx.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fehbvm.com/Article/details/glcoujoox.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.zdbjq.cn/Article/details/gmfayjvhp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gabvkmdme.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gsprskrpu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gqolsnctq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gpyislept.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gnfmzbfpu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gnqggrffh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/grrrvivxq.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gemokwqzj.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gkqpugtam.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gwjjxpwxe.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gjzjfrnvh.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gpkdzntih.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gidhhebfv.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gzeqpijvs.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gffpyknog.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gygrmcysg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gouhztjnr.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gyegsyjaq.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/godmnpyqz.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gikcydqyk.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gnyhkcsbn.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gntethtrd.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvmqkgxy.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/guehfobuo.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gkbljadww.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkkhmrvzm.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/ghmurmfiw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghfrouetp.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gnyoslvge.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gtwiveznb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/grwfolivs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gauswkpwg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gsyopsfbk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gmyhajdra.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gkovybedi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gdtrxzfpn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvomyudcn.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gzgmhtxja.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gkapikcuv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghzyzidww.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gxqcmcpyd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gakcasqon.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gvysmizxl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/ggyemxsid.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gsrumtauo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gcteilmgq.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gveemeyin.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gmfeucjhk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/ghwjnotqj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/guuutcksu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/goujblkbs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gcyobdgnu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gvrhrzriq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gyaintmwk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gixwkpltz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gcrgvtxaw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gsfkhtjrz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gcmpmhoxm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gqwjucwhn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gephgteql.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gdxkmzzcf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gktxgfnrj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gzihwquvz.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gnnlhvvbk.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/grnsqlkgv.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gnoaggalw.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gxihvpdhl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gebsloaiq.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gbabutsvq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gqxjkmsbr.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gtzebccbr.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gachkksly.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fehbvm.com/Article/details/gufqyzetd.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gmlqfzjcg.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gcrzamqoj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/glsyhnevw.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gywpogwix.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/goalerkll.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gabhskxnt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/guoyrrcdo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gprtrcqps.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gnqutarsb.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gyyjmrktk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gdvpkulbo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/geyczjntm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gnsvdsdey.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/getuoipmk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gognrerwi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gzdcuoonk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gjlbifkmp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/ggaryhari.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gsxfkhoad.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gwwovghil.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gvijusyih.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/grqlzeenm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gopuxlfkw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gajqpiayi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/ggmpjfdps.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gwktbowma.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gdmypbeif.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gegoyzqhp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/guejtmjsf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gpuifeyuc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gfyhgkydg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gbgxzqcla.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gawnyhpnl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/giwuctxib.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gucyuqarv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gtbtroxlg.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/guukjujdz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/garpabvyx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gcahcdgkl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gckirkwwd.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gatbpvsah.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gvhdpsdtw.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gfoohtziw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gvutvlaey.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gakljiuma.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gvjwdwakw.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gfxfjcnon.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gqyybljjv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gbmcpvean.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gzviarobe.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gfcbhfpyp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/ghnqecfow.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gbzybfhye.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gktvzkjru.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gfvdawgwk.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gaxugwcff.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gvmmojlnv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gqizxqatz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gkmkgaopq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gikcqkzsm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gguwqmzfj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gmmzgeqgv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gpzazkxmg.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/glylsblcv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gmcxcfigt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/glrahxhrr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gfzmnbgbn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gsrxjfupa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gxlwjwkta.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gdzlbkgeb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gtwuxlfhr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gjmfealec.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gjfdqdriz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gexfqwvpb.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gfhkpwdbj.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gyyukpdmo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gcfvnkbbh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/ghlkpvijz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gdhhzidqt.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/ghhduawsz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gzzmqzxkx.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gagovsnur.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gihgrmddt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gdbitjeha.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gigxflqyz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gfjkvjguh.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gdwfornsa.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/ghlqpybid.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gyhsypdoe.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/ggjtnaucm.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/glwojgolu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/ghhxnxgme.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gcjfiebec.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gbazslnnr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gfpdoreyw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gaqkumtpi.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gqxelhset.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gkuzfswtb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gbmqlxcnt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcpwhzyus.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gpppbazdm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guklgrdei.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gdahwvvzp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gnopqkfwm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/giptladwm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/guwfqesuz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gjfszuzjk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gtyonxbvw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gyrdvadsf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gipkcuptl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gyoikvpto.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gaxpfmasf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gdqbpendi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gowkuykda.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/ggupspckl.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gokjfbehg.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gszqavvpv.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gipvucljp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gdzxivppr.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gjxkcudki.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gtuzsgoca.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gutvcyhrv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/glvzduuyq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gbnfjgdob.sHtML


<!-- 参考信息 -->