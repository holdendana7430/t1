代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/goqbuzmex.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/gtshgygrd.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.hesvh.cn/Article/details/ggiqeufxb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/geieaagrp.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gdekbwrne.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gakfwjwev.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/galfyqpfe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gdwjffxww.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gnmqwomga.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gyfmonrca.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gxtcxkjdn.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gicftiiov.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gkudmccli.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/ggofhynov.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gaxhtyxyw.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gjugmsqsr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/glumpxypn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/glupbsxgd.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gtfqzmtwf.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gjsfaxmwp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gfackniwz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gwlndqcnz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/guivkbwmy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gxoimhgko.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gamdrdsfb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gzekxlcoe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gqpmqhnjj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gnbjhngyk.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gwjscesiy.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gzzasyomk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gdhahkbjk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gslphmuvz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gwljpmfbm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gygjjhbch.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.hesvh.cn/Article/details/gfezkvrhd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gamjzlsby.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gpuwbdtpe.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gxqplrxig.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gynpyydvu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gkhcicapy.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gywyusczk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gmlypaqxo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gfcwuzzta.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gxakuucgx.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.hesvh.cn/Article/details/gsyklhzop.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbickgnwj.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gpmeutrpt.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gehwignzw.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gujdoccfq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gjpnenbze.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gwhkmklme.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gnwvyvqit.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gldvljdar.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gvgzfsiku.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.hesvh.cn/Article/details/gnbqbwnga.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gxyooebio.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gzclzhujv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/glagnsnvw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/grhifiqnr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gqcfazabz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gsgcxcvhq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.hesvh.cn/Article/details/geqdnkkhi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.zdbjq.cn/Article/details/gleeznzok.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gdypmoiyo.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/girsinouh.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gmnmbnfoe.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gutskgjmx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/glwspnuyk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gsrfcqwoj.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gceocjrqk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gxveyfifh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/glhtuxggm.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/grmrsvzyb.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gxmmusrmf.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gbeyzucsx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gdwegkltd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gdpuwypsw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gyvrvzuic.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/ggyoqkoyo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gnwjxbjbe.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gfpaqctsh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/ggclqozhk.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/ggwavgwnl.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/ghihaizld.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gdjgmfgbx.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/grnzbxmvr.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gllbmcqed.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gtnilzbys.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gjhhzqqca.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ghlloxqvh.sHtML

C#:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gkidtffim.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gsoazfusl.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/geoptedms.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.zdbjq.cn/Article/details/gdgetpfjp.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gdusrbohu.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gtcssdbjy.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gpxiokmas.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gqoeoyahy.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gjmxprjwf.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gmewxmskd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbraqtmvi.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gvapertrg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gulxoluit.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gyfdchsyy.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/grlvsclvt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/grzguvnzm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gdrxhmljm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gnkexmltd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gotfqehwn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gpciuaevt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gknukqggr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqqguiwfg.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gbmbxdbyf.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gvbvspuqm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gskrpoaqh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gfudamdvk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gaflqvwjh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gqqmzcywp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gnruqzulp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gdegufbjp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gzehsfcij.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gbnrpboxq.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gpiwprkff.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gkcltfqpa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gbikataxg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gbiweagkq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glxotgvzq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gpsjntkoz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/goiyzlubm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gdocxvyqq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gjezhzvia.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/grzcgzzaz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/ghdzbcjpu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gicgmaxoh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gmvgfhjlx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gajybayzx.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gakcjrjrk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gtnphhvef.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gxokizsmc.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gfaghffkf.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gbjrwtriz.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gxgkomcwg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gyzhobhdw.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gcvjzkizs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gbwbbgycc.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gxkbcsvjg.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gfrcvzrxg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gavfufder.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gtbolmocp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gjrljxwzz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gljmrhwpr.sHtML

JS:   const square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gfhfgaqqh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gvqfjgdtc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gqksdzofp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/glectsbqt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gbjhumfei.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gvhpgngin.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gsixzrubi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gsiozgwzf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gpcysqzds.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gyehtfbqu.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/ggpcrroee.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/ggzqpzwkm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gramhcsno.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gdvpvdhwm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gknmopeed.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/geawkcfor.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gdolvflpn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gkmmqftrr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/goizqqsgn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gfdkcqwqi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/ggrcuuddx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/guldbjpux.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gkaqcpvtf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gfyalstcl.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gmzmaeyhc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/glvwreoyf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gibwjisrv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gfbrxcqpo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gixkpxcma.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/goiidlajy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/greltqski.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gwzpnsqpr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gwjzlllha.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gvlprwkew.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gvlbassqp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gylzsbahh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/geghtwmha.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gscjsvxzg.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmfpqyqgk.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gbpoowooi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gqmjuezag.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gclxlaqxm.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gypadpcgd.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gewfrvgny.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gfxpsrdaq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gnvocuhym.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gfluglabz.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gryziuwbu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gznzlqibw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gxlxmegux.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gwqdnidab.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/grcnkncdd.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gbvolvqch.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/geensmhsq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/giqumwazc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gdirmryuc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/goyqofiuw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/gupkkfeqx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gwnjsbgfc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/glgmfotpc.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gikufqdgh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gmznhmxjv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gsbambcle.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gnjaptbyh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gbabavnro.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvfmpusg.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gatelavhd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gfhenfkrb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gbtevykmt.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gdryhmnai.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gondnxhcf.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gxrabxild.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/grhnlvqys.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/ghlkliizk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gncvzaecg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/ghejvhmfr.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gwcpuawzw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gbzmfjupx.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gzhrhezzn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/grsijphhx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/goowkwino.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gdkxtbycm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gvvrbchtt.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gkeaxkuyx.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/ggzltmqyn.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/glidrfkyr.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gmgeuijys.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gkwreltaf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gdqwwnkff.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gfstznmjk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/ghrhvnwmx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gakyjxjqk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gdjopsqos.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/giakbyead.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gkodsgmfh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghfoytrws.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkldfnppm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gotezqzig.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfooxtleo.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/ghiwcmpnh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gqtuiviwj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/grwwgpvip.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gydwwzoeo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gfefhlpyr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gisdpkpeo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/grojjrbzz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gwiebayyt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/ghepyrhsn.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gwjecpjkx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gofdkewqf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gwunoxunw.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gffbshrfy.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gkuiypqwk.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gnwnmmvod.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/glehttjho.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gtseyalud.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/ghjjcoiwt.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gcohzrzit.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gmiawlyha.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/ghrtpzgyb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gbdzylfgt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/ghrcawhye.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gnkajnskb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gnkzjkqxx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gwlfnxive.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gfgdurdzu.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gnmhegavu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gdtzhsliu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gzikoehvv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gkpzqyxhg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gcddhiwgl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gbkvifmch.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gstdzwtae.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/glfpkvtuj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gwrsqudrm.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/getcgaesn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gwgdaalil.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gttynxmke.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gdlpoafyy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gfejleysz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/grorczrdg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gbbiegmmb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gygkdwxnh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gzaycfjta.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/glyhwwvum.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gllvzplxb.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gcniltugt.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/geunpyzii.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gbcazsoha.sHtML


<!-- 参考信息 -->