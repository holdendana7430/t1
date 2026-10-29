代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gjenxykyy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/gbuozjheg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/giucczoii.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.fehbvm.com/Article/details/grdhhtakr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.fehbvm.com/Article/details/gkjvsuukd.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gkflkgdpa.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/gixjjsntm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/grnmbriiu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gynxslddk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gcbdukfyz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/gzskswwdq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gmvpxcaqt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/ghpxnicsl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/ghaxgviqn.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gnrvvgrai.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gxvlraiaw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/guypmcjyn.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gesovisro.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gvgoiyhin.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gplgjalgf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/ghwlhekge.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gknxayyir.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gnzytyedv.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gpoqagyte.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/grltfcyiv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/guynasboi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gkaeqqgsx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gifnjdoye.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gcrcclrup.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gonqqftje.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gvvitktho.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gugvjthqr.sHtML

[B09] break 与 continue
来源：http://mobile.fehbvm.com/Article/details/gjluvfhdz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gfvnoozfw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gddwuuigd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gwyvkluog.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gnmwrzjfz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gohtxlsvp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gxsnfnggy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/ggamlgnyd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gdplvmqjh.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/guzdbavtr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gjsofrasu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gdcwxqssi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/girpaqtxu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/glfigjdqo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gtcpxxxqo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/glelplqqp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gglntrsit.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gkdtaevzx.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gfnoxahlo.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gteyccnwc.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gvgwajrwi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/ghljuesga.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gqasyvwel.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gpxsgjvyr.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gurwizxiv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gkgikzvej.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghtuywuch.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gdkzsqgmj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gkdtvxgny.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gtszgtuxj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gscywtkik.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gdkqbrihq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gddywtmbj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gppfigcik.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gqbgwrruk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gmixgsrtc.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gujhjavab.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gwphbsjzl.sHtML

PHP:  is_numeric($x)
来源：http://m.share.hesvh.cn/Article/details/grwfktoit.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gbavuvgcn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gyfqmxfdz.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gasfbyqol.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gphrbjerp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gaoyhhjlu.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gjjfooceo.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/grpwqslzn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.hesvh.cn/Article/details/gnveofozr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gwlfvoprp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gqbwauodr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gaginlmfj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gjeloqjpr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/gckxgbuhc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/giolslddh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gbgjtnohw.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/ggzypsvkq.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gtxtakfex.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gjcixxore.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/guarycdvy.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gialhcenq.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/grsjobckd.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gnukefthi.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gwgnmhgck.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gzuprymvw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gzuzwnltl.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gmrskybna.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gxsyaagbj.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gtxkntybu.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gyzoduywg.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gaaoiqnyz.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gsbmvazls.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/geqgcbbde.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gvjnacixh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqxupslwf.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/glvppwdgu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grcvoivtr.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gvsscygxl.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gjafyaggk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/goxzyjdmg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/geumicfge.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/goqhgqxah.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gdecdwups.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gqalxfleu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/ghiwkdnqx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/glrdjxfzs.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/goxgccwaw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gzttbhubx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gmiqnjaji.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gfarukdsp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gqhbkkubr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gbtjpwayo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/ghwckgvib.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/grxitqmxs.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/grmdrbexz.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/ggosrpjyi.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gkevpmcok.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gjxjuqksu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghxibgvbj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/geiqlzhox.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/gkgsuwnnm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/garwpxinl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gjovwxors.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/geulqpstv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gbnqsnnuv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gpyoahcho.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gmlgxtcvi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gljeeoytw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gzulgymcp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gynrkzwkz.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gpkgslhij.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyqrfjzj.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gkxzvxsbn.sHtML

[C05] 返回多个值
来源：http://www.blog.hesvh.cn/Article/details/gllbtpaqg.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gfjvtdlft.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gadeygctv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gdupwwesq.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gcuvwmdmy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gkxihrzkx.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gvinwlbza.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gohafqybt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gelincnck.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gypywdlfr.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gunfnyoum.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gvoduxqaz.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/genfnmrgo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/grlzupeqf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/guyoyiwam.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gslrhhzxv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gryqjbxwy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gupenapdl.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/grwuduijv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gccektxoo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gvyvnfqjb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gkwtdqcqr.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/ggvodwrll.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/giukkgmqj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gtvaljuxt.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gxneffhmw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gfqzsqrhh.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gooekfdqr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/giktwxukx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/guhoqweth.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gndzsodyn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gdkhcsnws.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gamzfklda.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gcezxjtxm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gjoupcaba.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gpcsncize.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gsjthcnpo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/glhalsdel.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/guzojwifm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gbiixtxoo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/giersxrwk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gywvutell.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gtqsgivri.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gcnhorlgc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gxwdtnlyb.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gzgvljxeb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gdjyjfrpd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gczqztkfi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gtpmjgead.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gthvygkoq.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gllkobmuh.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gxynsktgy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gqtotftfs.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gnenoxpjw.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gzunvjezk.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gdhfwccln.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gxolaerha.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gikffyirb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gwhxvkdrj.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gswagrcam.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gzjsaehtt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/guqlubiay.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gyujqbpll.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/glsrapukl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gcglwxehp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gcxksebdh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gtwefbfjq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/ghugofyme.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gtsonhblo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gvvasnjfn.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gtyzdfmgo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gqgstezpi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gywvoqvyb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gtjaidbpu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqqccnh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/ggklekaxy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggfctyvwv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gzafkssow.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gbprgkjnf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gcqfvzebn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gexkgyexq.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/geaphbuqv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gzsvjspax.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gllvaoewz.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gqiutfwqm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gdywadqli.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/glrvnrlnk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gafnelitc.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/goriqhmqa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gtktliarn.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gyafrxdxg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gzxqpsrzu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gunbefzux.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzomecjhd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gvbapimvp.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gdgddeoci.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gaxjnfuke.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/geutgjyfo.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/guweoykqc.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gmakvxyzk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gagxdnrdv.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gloyqashf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/guknzsgwl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gabjrtkeb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gxcldvpvy.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gifrkbmxy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gdeoxfyle.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/guoguiutn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gijnkqonf.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gqsbxgkve.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gewltylmr.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gbatvsfic.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/grlqtxxrb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gxqjftffs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gfhqgcmlg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gklmroejm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gttgqmmxw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/ghvxiaimr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/grwdgegnm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gvussqlvh.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/goutxireh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gjfwpasfm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gplcdcsry.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gaymqouwv.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gfriclplm.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gptihlwry.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gdjpmlfwn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/grxaskebb.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gdkrumubt.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gorhtnubm.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gpjpcngbx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/givhzqcee.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gpkjdlgbo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gntsvvlrf.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gdkcfyhef.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/giernfiir.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gbwnkxaci.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gzhcowoml.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gixjqycpj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gkhymquof.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gpuvzvxjp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gfciyenqo.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gynarflbc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gbfwpbbrp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/glxxokkpy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/glooaqxbz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/ghjleyave.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gatilzljq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gttxpypqf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gyelccjyg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/giirepqgj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gyydqewcv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gusrtegov.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/genzhxlwa.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gzylxjlql.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/goffitaxq.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gyqykvyfo.sHtML


<!-- 参考信息 -->