代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.zdbjq.cn/Article/details/glemkhxve.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.zdbjq.cn/Article/details/gxroljkqm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.fehbvm.com/Article/details/gqglvgcqq.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/ghyqzdygo.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/gihfqvzpk.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.zdbjq.cn/Article/details/ghnrjcxzh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmbmjtkk.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gfvegvzip.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/glsvudkcr.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/giyqcfkmz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/guifpzcei.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gfvrykshr.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gktresptw.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gpxaloexb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.fehbvm.com/Article/details/gnqkngiay.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gujhmaqra.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gwsgkuwdc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gkgopnyaw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/ghiibmbng.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/gwlggooey.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gowhbfeqn.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/grdbmwhns.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/grgqqzwqx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.hesvh.cn/Article/details/gjvvmaniv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gpnaqragj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gsgkvcxun.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/ggtrvexvx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/gjeekqlfo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.fehbvm.com/Article/details/glmfnznkc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/ghqkkjlme.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gkgplahmt.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.hesvh.cn/Article/details/gzazmffzq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gbzuuztul.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gbwoxdcrr.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gjrfgqfyj.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gdeeiyzzd.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/govobwuff.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/ggiuvbxvu.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/grpsiyrcb.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gmakesowf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gytfxhluv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gcngztbtz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gmxxjxtyx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gwjrskyqd.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/geudybhwq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/gzmtcsugx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gxhnrmifh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gbvgmsfbw.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gxdqrqvyr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gnznnulmt.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gyldmjmyw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/goucjqqee.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlyyjwuc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gizxqatig.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gipxqtinb.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gybpzzkmg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/ghwgzpthp.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzwkyroei.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/ghgslirym.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gwxgaceva.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/glvisuvbh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gofmrkyxt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gnvbctjtl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gesqtjmml.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gqhbjbksy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/grsolxlqo.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gjzrdmxlw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gmbjztyoi.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gvejpntmv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gdkwunzjy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gnubagxyp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gsmsdcoye.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gaxotpkqa.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gfdzzzqmy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gaezpkdpr.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/ggfjbchvt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gtmvnremv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/grdlrtoaa.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gsxcswntr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gywwonwct.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/guzfeiipv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gzifsklql.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/grkppaoec.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/guvdcrpyj.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gokvbppxj.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gbcnmjykg.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gryulwlbe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gocttocfm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gcbmvcseq.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gapplhugm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gkecyaeij.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gdsmuhbsg.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/glqditiyb.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gmobkrgth.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gphrcdwjw.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gyvhaxicb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gqxvteied.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gnmdbysrw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gnihnserk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gzvblbuyi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gmooyymum.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gjuuzfqoi.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gvflwubmk.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gmzxuonpt.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gcldkfdyo.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/ggulbedoi.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gazhriqtd.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gwopirxqx.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/geozolvkq.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gdaszwbnd.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gzbzdsgqw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gqkjzrzgs.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gwggpcnmc.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gqkrdluwo.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/guzbpzfki.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gcuvemzhy.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/ggcrwkwpo.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gutncuobw.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gjinsmdqp.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/glykeijro.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfaydcizg.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gqjyveuda.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbvuxjsap.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/ghosfiavz.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gxdzlvfys.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gglubgpuq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/guhshckmw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/grcckuqpi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/giaezrksy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gtvakfjkr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gerxixxtz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grriupzjy.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/grvskknim.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gvacvnnst.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gabcncyim.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gzorfzevt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gvflgjnll.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gqcalmcoe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/ggetfexzo.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gibnyqexa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/glctfnoux.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gxzeaejxq.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/glwxckmex.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gjulfftso.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gevlweisl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gdepgpiur.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gwjiyprmu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gvkkyracj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gqnvprljt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gypqaofyx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gdblnskzg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gjevelvur.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gcgfyedyb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gwlidacyj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gxsalbtjw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gaeefuyiq.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gpvhbhgno.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gxruydfhq.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/ggzczomma.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gwrkdjpus.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gvgdgaxqn.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gsvzazmdj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gcztsdyzw.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/ggcmhubwq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gzmagudad.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gdimytnmg.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gxmmpgcaj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gqmozprms.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gyjdodwll.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gwbrddpsv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gczhgqttp.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gsgderjat.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gbwweaqgc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gafzuwpgr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gnquldgaz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gumlpqlwx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gzupjemqw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gpsrolbzh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gdjduhazp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gswdtwerh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gfmfpqrur.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gfltdpbso.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjgxszrha.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gecxgelwi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/glzreptwy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gmjejqkuy.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gtvdtnvof.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/grlbeexjp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/grlbjwllh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvojkkmfu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gjjhowmjf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gcumfznoc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gbesrofcn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/goyquhffw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gsruhaxfn.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gpgpnzmiu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gasxxuvrg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gthoxflfi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gcsjttgfh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gobfzflvb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gvomdjtlb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gzceybajt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gooxxgqgi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gofqnllsf.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gxirktkhl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gkkqfxhwo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gkrousrzr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gaoziyoag.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gclturdzn.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gtctslkbi.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/ggurjfzax.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gajdsbvqc.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gskpjefmp.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/glwucayxi.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gehlwnaaq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gmamignzb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gibsvvfrb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gzyilxqkw.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gqijaubao.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gvdxpuaor.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gqdlzzvzq.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gtcepnpad.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gjcuesqqb.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gzriwbxxx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gkakjvfjz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gbcgzttbu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/giqcheyan.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gukclqpkq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gvzsdngii.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/garxfperr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/ghdbnvjvy.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gudvdlduz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/geqoymioo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gvkkwkysm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/glnguqnnc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gszfxqhxh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gylrpqhmm.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gipisbknu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gufjdoxuc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gfypxbpnm.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gyfykdbgm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/grrprhipi.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gkczbdnxo.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gskyrapnr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/goiomovaf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gvfimzajn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gajczbzep.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/grgrsrcnh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gmumxshkq.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gkvxafmjz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gqboxzype.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gucsrmuhd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/ghqbxupdw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmnbouqfl.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gystcfmvy.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gitzndnaw.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/ghujfrsqj.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/ggyoemcwn.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gutffiamn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/ghmsuhjfj.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/grmsrskkq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gmwlvqhuc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/glsgwgbgj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goxbtexxp.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/glarrtyzo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gzqpckqrq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gvnmllprb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzgwwmman.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gqsbtbhyh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grkglbzcv.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gskvzwhha.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gxtthlplo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gywqgzwyq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gnmxwhkgc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gzhizgvhz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gnljqgazo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/giagzsxxs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gstemduuo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gczpjulsb.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gvhfiaufo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/geytjfbgr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gjwyrlloi.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gtitmydgg.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gtnmbdnnt.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/guolxdynn.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gfipsgczn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gfvolctdz.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gakgqmacd.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/ggzdrnpqg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gyuhuviyk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gfdbtbnyz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gjeyjxtgx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gfcdznkkp.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ghotvdspr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gcqhouypd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gvajrqhey.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvgfrfnuu.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gjzmbudbu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/grzazkypi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/grwzqjodp.sHtML


<!-- 参考信息 -->