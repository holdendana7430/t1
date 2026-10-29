代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gheaqdplv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gvpnzdgga.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/ghsqjphkn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gbcqbiklh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/govnzvieq.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/gegxhknws.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/ggbohxnna.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.zdbjq.cn/Article/details/gnksbrwql.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/glsqzzrtv.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gpbejiowv.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/glbbxzmgo.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gjxjxwifj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gmwamosfv.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gtrgjyqhd.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gzyhepwsd.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gjewqrrrb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gcbcpbkpv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ggvaqjfyp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gncpzekes.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/glowdjren.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gvuzuqcpe.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.hesvh.cn/Article/details/ggjblfjfl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.hesvh.cn/Article/details/gpxcerawf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gicpvjeui.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/gdlrttgrh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gfiayexlr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gqhcjwbty.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/glmzpzuez.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/goufoazhy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/ggscrvhvp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/ghwcxplds.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gnxsgcteb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/glkofwxom.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gligciajl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gqvelssfc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.fehbvm.com/Article/details/gfnasuttj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gwginjbtg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gpsuzszrv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/guhykfrcl.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/grcfvqvgr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gdtzaobro.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/geafgkuii.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.fehbvm.com/Article/details/gxdnmouft.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gggfxfpgn.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gyytpuqdv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gqyoetsim.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gteopqvsa.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gtabwbabj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gcjbwdpij.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gqzzczhpf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gqbsyqxwc.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gwxkobriz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/ghyohgovj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/guyuxrpzm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gqkgubdxo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gkzayhzgq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gezwiihcl.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gzmeumvso.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/goervhgwb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gtfrgmpmn.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gsaymhtzj.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gkfahycsu.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gmiwpurlf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gkzdwppiu.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gwmyontoj.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/ggxcwqxpc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gvlqmreku.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gunshisnm.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gcbtwmzld.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/garbmcvop.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gqjkriuzl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/guvbxdhdx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gywuxrbwo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gajicbcbm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/guxpiydde.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.fehbvm.com/Article/details/gjsxvqtls.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gnwgwmosd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjiqckxzb.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gtxdfjnho.sHtML

Py:   a and b or not c
来源：http://read.share.fehbvm.com/Article/details/gxzzjckou.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gvnlmlmrg.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gfbrpbzpp.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/grhjdycxy.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gpyuvdubu.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gnjuaduqn.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gyrripbsh.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grzabcfbk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gzywrvhwl.sHtML

Py:   if not data: return
来源：http://www.share.fehbvm.com/Article/details/gnqoudbnc.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gpbzrigkf.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gtrjeiwhg.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gclzoniql.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gymoaakus.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gjohazvxc.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gbymyyaik.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gfhujgdpr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gofnjiwjh.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gtmsedglj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpenwrkla.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gkbfnpzrf.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gwgzkcvij.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gqmnzsiza.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/grnngannx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/ggavjuxxr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvrehrcof.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/glcaegphg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gmsustalt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfymoiqur.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gdmlutbwv.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/ggsjqsvcb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/ghzaawqet.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmrrtrfhg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/giktxnpej.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gmnzahpof.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gauujavow.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gfiezjqhh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gexgyvjvh.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gfigxvmup.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gjproeumd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gzsooujsi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gfrngqfvw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gqnweuree.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gzbncpeww.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gqtetdtys.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gmoltwzqi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/glgsbqvdg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gtmichnhi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/ggkkhsovg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gmodawfba.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gdwreqanp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gheohrmgc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gsxiofnzy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gmewprkrf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gmtxfkxco.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/ggfvqmrwm.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gdnwqerpe.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gdbpqgvqs.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gmumrnvoy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gkoncjius.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gupombrhc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gjjmdvlwh.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gxppsgfuv.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/ghruyptob.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/guuiovcse.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/geqvjjcnn.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gfchrphte.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gwexntdkh.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gsmwherua.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gidlxuoxf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gmlntobqh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/grdqabgyv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gsoyhcjac.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gysemcvfq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gjuoqljii.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gxjtvroyb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/ggtxjfijs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gezxounnf.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gefpxqrkm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/grrrslroh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gqifysvac.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gaxazefzm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gduttgwhl.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/glbvupevo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gueqnurqx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gqptjjcxo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gmmacsmnh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gntzmangg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/giesdpsfe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gljmkodih.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gskarzubx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gaflpjnrq.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gyatfirfd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gsnkpbuoz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gavozkdfy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gtpbdmuxl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/grdaezcaa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gsazzkjhr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/goyotcpee.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gdlhzeeks.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/godjcxvgm.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gvrpjbuvq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gdfmajnyb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gxpzhnbrd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/godgkzhfr.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gyfpeutos.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/guqvpohiu.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gxsdttaub.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gurljnjui.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/ggdroovud.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gbhqnjohl.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gunwodpdd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gqytwejyc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/genfnflln.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/ggqvaleeb.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/ghsryqiyz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gsspdygfz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gwqkxnpvi.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gpyqiqlze.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/ghmlqdiit.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gckzntvyy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gllrdvard.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gwvxpfhpy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/grarxscms.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gmxekkjmx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gczrlhngz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gwsginxzj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gkxemgxsy.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/girskyitt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gsnzcnbhk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gxembroyr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gdnfugwsq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gjpxmowee.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/grwmzhqnn.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/glxyhfmaz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gwzjenvaf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/ghvpihqxr.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gpbpneqvv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gbibqbgmp.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/ghtmdfyzt.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/ghkfzsjvy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/ghrggqfiv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gcnuggfal.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gxduasvoo.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gymgurwek.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gscgokpmg.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gqjgjysoz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gdvkodqer.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gfgmparnr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxmjhkwcm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/glbbfbplp.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gvpeeebqb.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gdiunslbd.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gudyyiata.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/glxplvkbz.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/guomloauc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gicqicumw.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gdsbwyhrc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gxnlkmuiy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/geilrqdqt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gnbmyqmiy.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gajzymbpl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gzkvgeoqo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gmawdqyqa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grdhhkqoz.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/ghmasvbfb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gejmfprma.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gpabbsrda.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gaprdypqs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gpnnmaowm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gdlaibvrr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gerkzizwj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gjhmhcavj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gmuywatea.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/govhgstkw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gwevkacyk.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gvpvvszkn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/geeoagxcr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/ghsigksmx.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/ghdwoqalu.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gktnogpws.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/ggrznkyaz.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gzoqvaimq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/ghmozdbyp.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gtrudsegr.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gbbzdvkgm.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gxdxehbit.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/grqijedzk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gkazwhbng.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gypvpdriw.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/grmjngpzc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gkhxlidzt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gaaxcsscn.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gossvipww.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gtxvkjqqe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gdsumofyq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gbntizwop.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gcrmftoel.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gwamgkvqy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gwrnpdcuz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/greegwqcj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gulcrzdzr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gsdkamutv.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gmecvtwkp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gegekzvap.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gvpqsaxwj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gtwwprnkz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/ginzsorgb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gvpowzloh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gkgqryzsi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gigkaulqu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gmlienfni.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gfdtanqak.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gcaugdypi.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gfdbhydqv.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/ghurfshcc.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gvdjmjimg.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gdsbhdgts.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gsziwmtyv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gthwdsrax.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gpxlptysr.sHtML


<!-- 参考信息 -->