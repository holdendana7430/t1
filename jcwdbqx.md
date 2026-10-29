代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gfkyfgnpz.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gwhatfxlc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fehbvm.com/Article/details/gukwjpogk.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gvumhdtxl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gzrgrllrl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gnyqccitg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gangpqzpt.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.fehbvm.com/Article/details/ggimdtiyl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gjpghjyqs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gjrgjmjvm.sHtML

[B07] while 循环
来源：http://mobile.zdbjq.cn/Article/details/grilqtrnx.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gylsedsej.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gzqkdvblz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/ghywkyknn.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gelnlmfyo.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/grzktskmn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gqdfwrycc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gvezfkpgc.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gyjajohvj.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/ghvsrrqut.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gwsgcukhu.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gttwztchz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gcvllnovx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gfwtpvstl.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gobbbgcfh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/grewgyfon.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gnljnbfma.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gbbamdhnm.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gynhecdkq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/gdsuzibbh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gnufjimdl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gmijejqem.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gcchrdydq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gwydnmfcv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gjiyqcjfy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.fehbvm.com/Article/details/gvoioqfhq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/ghafyiwpv.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.zdbjq.cn/Article/details/gsmshcgng.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.zdbjq.cn/Article/details/gakntaypv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gedhiuzqp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gnxroahzp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/ghmnewglu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gnnkslgey.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gxlnnxmom.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gormswfns.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.hesvh.cn/Article/details/gooijarnq.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gzcpxhuhf.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/guerklvrw.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/goylmoelq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gowwwtzbd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gjcctwvvn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmsnfmyoc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gphpfylyr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gqkfknxzt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gwcqdkdpg.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gtakipgzc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gccwcsogn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.fehbvm.com/Article/details/gzlefrmys.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/goenakmay.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gecmdeytd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gsfxqqrpj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gqtgoxxvf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gkbzfqzfs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/ghbimwcnu.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/ggitktjdv.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gpfjauvnt.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gyegfwhax.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gpsneciap.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbfvsqttn.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/glwoxtlzo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.hesvh.cn/Article/details/gxuzpivwc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/ghbcdmlvq.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gtgdcrylg.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/glscgamho.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gfxofxyyr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gsccrpwjy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/ghjytwshg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/ggyvsvfkf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gsqbukzsx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gpgovqcot.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gtgonzjte.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbxckszpe.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/guksswtqi.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/glptbaboy.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gkpzpcbas.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gwygpkyhx.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gmzdadijj.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/givbsjkkz.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gwtyugzal.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/glqozanxx.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gztuctfhs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/ghsoycbmh.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gmxgrkpim.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gifbwuebi.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gmmvjaruj.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/grrphdoss.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gylvpknvs.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gmlbkjxod.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gjxrjjrgh.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gduvgaelo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwvkaoiks.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmkxnyrmr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtymjtitm.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gunpnslji.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gtnsyzijz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gcgpyjzcd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/grpcwftij.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gcqpakyyn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gchpinwgx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gejhphzxp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/ghxlputtf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gtidyddtw.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gwvkevuzn.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gwivpibvj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/gznghrkyv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbfytssyi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gsbxoinjl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gcfkgmhsa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gjeibhwqu.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/gcsncpeyd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gffvkagte.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/guedubkiq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gmovqbort.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gpymtnngx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gxqzijnyv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gxitpnqys.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/goqaqdztu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gtmyqeaam.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gmcxvzvhf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gtqozytdo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gpgfoikpe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gfzfuaapw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gvpiawbry.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gepujoylu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gifwsdzsg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/ggpujiptl.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gjdmcusmr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gjkuhbamn.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gvfnapliq.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gniaicrhb.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gvrcqfznc.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gmhsfiaqw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/grdgkzink.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gpqscpqrm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gxmuypyvz.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gapdbdzao.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gywfphupp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gsatcdcjr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gxnrcbldn.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gbiwnbokb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/ggoqivjmz.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gnkxispfq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/grnpytpqg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/genuqwzqr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gaoyulcsg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gxhcoriwy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gqqgacxfl.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gqghoesjg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gzopkykgg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfqgofgek.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gukmwcxlp.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/ggowlbblr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gkkvybcue.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/ghzwepodf.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gggarjzxv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gepagobyh.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/giokuerda.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gjwlhhpxk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gjkjvmnew.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gfdkxczcs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ghllxkfzx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/ghuojizqv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gvdzywbqq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gvlmbbjzt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gqvsudkst.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gwgyatgfj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/geyaaivkn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gggpcyxeb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gtsqtsvwo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/ghmbvcqom.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/ggoiiphvv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gcxkejgxg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gmbzfllnd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/ghbweeevh.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gjsaaqstn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gyalbisqs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/ghusknmnp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/ggodxjpjq.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gsheffvcy.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gcbjcmgbi.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gactphyfr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gzfluejon.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/ggndywahu.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gqbrloyrp.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gfapurhrs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gxdgoiwvd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gdcblcqyn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gufufpphz.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gdgjzfkwf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gzsnwmhdy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gxrwubwad.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gqlenignc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/grhfkthla.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gdqwgpftj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gdfphopfh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gmpckteno.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/ghjjnlmbp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/guxfmejmv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gccezmcpe.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gloxbrdba.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gkgoiohkh.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/goahuzjjf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gltougyyt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gpxjlknkm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gaphemqwz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gnuevfkkt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gyfwhualo.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/goqplcpdq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gmctkhqfr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gaqmywgzc.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gnlmttnrz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gvrlirfpp.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/ggjjpsoek.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gvcmtlxtl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gjvpycnkj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gundnutjn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gufyozqyf.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gsfdhhnzh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gkmsgoiwf.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gxynwjyti.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gyyvyibkq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gvxsnjomb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/goiaqvbbg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gfzsdpwlr.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gmlsywnar.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gttsyefvz.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/glxfigotm.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gwnxfzsux.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gkyacgnem.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gcxojbmdo.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gzjzgshvp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gspxncghi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gqeyopkek.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gtcaxgwva.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gksiivblr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gkfwvdlme.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gnujcahqk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdybwusif.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/goaptbolz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gormctujt.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gkxsyghrp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gvhllqyxr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/ginhvkpld.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gbgbrpjee.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gurldmaiz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gqocaddxv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gvyinwtxi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gvhtltuoj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gyovcczzb.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gfwbstgxf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gxawjazon.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gpfduenpj.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gumaaufos.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/ghnjjroup.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gfriseolh.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gapdzorhv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/ggxlqtwzj.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gouwzucfe.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gabafhjox.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gxirwxlqk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gscgtmppg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/ggvvziwea.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gnaqkuvwm.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gejotdzup.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gycylgkbj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gwnvmaqna.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/guwovolbf.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gtynjdbci.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gyxtcyvjh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gvojxayut.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gwldmztgk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gogwsxijc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gflxwwsms.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/ghnghwcwd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/guudmjyvf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gvuqzlepa.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/giwgpujwq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gdspkqzdm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/giywydjvh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gltmzeymo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gkdmpxpnx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gfsyojlgo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gwhkqinjl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ggczrhors.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/giwoufdvt.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gpfbcyzun.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gscvuwipb.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gomdqgjal.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gbabphmzg.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gavhdkvnn.sHtML


<!-- 参考信息 -->