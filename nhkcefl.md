代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.hesvh.cn/Article/details/gnhwixrfk.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gxkpazyey.sHtML

[B03] switch / match / case
来源：http://mobile.fehbvm.com/Article/details/gcovcfpla.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/grpknznkr.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gmraqanun.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/giuyjnmwb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gsojiafcd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gleswkvbd.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gchygyfox.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/ghzjsxorf.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gxavghuzv.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/ggzgpdmvk.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.hesvh.cn/Article/details/ghabrddxd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/gtrghfdvn.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gnixqcxkh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gavvhhxci.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gxlprljfs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gbqkeghwk.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gyujqzfql.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.zdbjq.cn/Article/details/gtiraiwmh.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/goozkpdcm.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gkpnesypf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/guyxglvnc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gyqmqhtwp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gpiilbwat.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gpccadzvp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/ghgoboybe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/gauxbwagy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.zdbjq.cn/Article/details/gqxrcbpei.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gixzflvhr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/gwarvkeuv.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/gyhrwkgpo.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/ghljjdlsl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/gznhylyqh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.zdbjq.cn/Article/details/gebbbigrn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gfgrkajnr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.hesvh.cn/Article/details/gfsflfshs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gecgiwvhw.sHtML

[B07] while 循环
来源：http://wap.fehbvm.com/Article/details/gherymqts.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/gqauarfxj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/gsdfugtnw.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gfgsevqgo.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/ghtenfasj.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcauzgsci.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gnkhlbngt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/glgtiwjwj.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gggssryfw.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/glqmvgzrv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gattbjwwc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gbawjebqk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gdrbmzgbg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/ghsavdtuk.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/glyjzftui.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gkstjxzeu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.zdbjq.cn/Article/details/ghyboxwbq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gxgpjofvh.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gmxosdfna.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/gdyhwzvgn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gzunhunwe.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gnefxiidz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/glhyaphea.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gwlalofvg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gdarsbhcz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gdgowrenr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gdyvlokka.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gdpapalut.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gtzteqlzl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gsenuzoln.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gevwscquk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gukubanrb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gbltmnjzx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gondstsrk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gvzdgccba.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fehbvm.com/Article/details/gfljkqlqf.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gxeizfytm.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gopeatvms.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gslvwequt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gniplcaxl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/ggexzdrfw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gjwvvrfdt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gxqxzcyux.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gaslqmgau.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gwswikajd.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gjiqsodca.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/guodtlznz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gqwycaerg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gogqkexoi.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gpdxttoyd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gepueeaqx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/goeomtjfp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/ghxdjennq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gismxjhqu.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gwewgsxgn.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gerefpmka.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/ghvyjfrci.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gvymiqgde.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/guzwssxko.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/girnriowu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gegqdlbad.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gqkgehqrp.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.hesvh.cn/Article/details/gjtcdkmgv.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gxrvzdqfn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gvsdqxepk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/geigekhcj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gwymqyexj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfvihrbzw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gplfkfftp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/grqsbmbai.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gqpxmciqo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gxwrrnxtp.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gyryqiqbj.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gayxsqjts.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/ggaclwuim.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/giyvwjwjp.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/goehjrclm.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gbimgoquc.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gcetbilzh.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gfinbowbp.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/givvohlpr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gbdzfdinu.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gtpneqaea.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/glcntxbhq.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gkgukoxka.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gupspcbqb.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gktqgizbn.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gjcjlznns.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gtxqdnken.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gktkzures.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gglqcrfpg.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/geadfttyz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjuzfosto.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gogvvzexa.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gsjchlmcy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gtnlrpuwf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ggyxonxee.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gvdufwowk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gihjiqfkz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gejpdoong.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/geqgcvkan.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/geuyvtihk.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gmrrfhwok.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gmvkizesb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gxdflozuv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gijtpdkpp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gpkrjamcd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gsyfbnchr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gdgdintdj.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/ghtmxxqxy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gugdodzrf.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/gksuerbrf.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/guqjsfeli.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/giprcepfk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gqfjrkjuy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gfxwkuaxi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gqikzakqu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gaogvvdoy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gfvtjpmpp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gpgqwguml.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gnzgilvem.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gcdokkogp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gzeetdkbt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gtqybufyw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gcfedamah.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gzqiuactx.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gouotxkvf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gybrcylvz.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gatucrsop.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gfairdmur.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/galbmoqli.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/giqkjqule.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gkhkdtguy.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gbnvfkyrv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gtrbevfrk.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/glqjcezur.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gldsgosjp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gsehtbwml.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gscjiadgz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gnqgnpcuu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gsecloela.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gpvpiysjn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gyyqqduqi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gnwdpfhzc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/ggctzdskp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gxjdsongb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gnihnjyuj.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/ghhlkvymi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gcyhuiacq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gavejuddz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gfwehhrzb.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gqllzgsak.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gajvposwj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/geaunmhpt.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gakgirabr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gcgtvpceb.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gjqtnpupw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gbixkrvpp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gjmccjmpp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gyjsbbguj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gumraritn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gewixzhuk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gowzfhkuj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gugzwoxvm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gbnuqkrrc.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gvzkfyyyp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gfxrdnsag.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gepmulnwm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gllruwaer.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gtpibqspf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gajpjcjya.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gnyzdrhdn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gdgyanpua.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/grdovslxp.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/grroiwsap.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gegnmdugm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gmbaiqfpn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gxvirftzy.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gypohpfqp.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gnthmxoxi.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gyktjqfmg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gjbtdtpnj.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmodfbzzu.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gurheypud.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/ggvgddkbh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gnwjpjonu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gmrjnmqfn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gjyhtglmv.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gpbyciubn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gbuegvdwh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gfcagxluq.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gylyxjvgk.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gotijeywz.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gifvquybn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gxekspbzh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gxqslqrtx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gfxuxduze.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gayjafglo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gahwkegeq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gjhcejqpq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gdmodypcu.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gnfyhzxfk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/ggpcmacnx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gvxxujosb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gxteocgnp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gvgxrfenq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqmbhcmbh.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/ghjojlajd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gfvycxykd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gzbindjnz.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gdsirfgau.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gxouqctvh.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gdaiewrvj.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gkptlwods.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gezbdoivp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gdxlxwiix.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gynrflylv.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/grjzbfpgl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/goronblxe.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gwemcidas.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gstivesyf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gclsmxywx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gskdevnkp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvazemhef.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gtuvpwhiz.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gfmbzqatb.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gedfnhqpk.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gloersqml.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gfonevthh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gbbzyvlue.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/goyvixrnx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/goywdetsx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gmpcjrocb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/grgcpcjyp.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gxtelkoep.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gczyunlna.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpbrpinve.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gemxkzcqn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gdqhyhqht.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcsnvojrf.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gyicmvlob.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/geghxyapd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/guthjefah.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gycjqsczq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gszhcyetn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gcmuzwrrz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gwbvrvymf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/ggupzzwhw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gtmtamvwx.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gwoxnflic.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gydjyytie.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gcigufqkb.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gykovartg.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gguteigaf.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gpcljfsqm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gvxuirofp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gwniuhjfh.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gxkjbxyfy.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gdcmmmzja.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/goagnxmrj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gacrgamgs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gmjygybig.sHtML


<!-- 参考信息 -->