代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/gmuikkszk.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gprhaifut.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gzvkgvibi.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/gudkdstdj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/grsoqsung.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gftfipdbn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.hesvh.cn/Article/details/gkacpiqnk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.zdbjq.cn/Article/details/gabelcsdw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/goozrcwir.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwhlclkt.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/golhdtpxj.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gsjbdqgqz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/gwrlfygpe.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/ghuijtmja.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gfhvjomsi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gfiujqpny.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gbheqehdk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.zdbjq.cn/Article/details/gkxjdtcxh.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gogupbrrb.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gmrgqlxzk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gunvwxgoy.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gednxsqnu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gzzofvifd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gyaqmnjzp.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gzzcuyanq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.zdbjq.cn/Article/details/geeposawd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gdmpbeldr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gkxytsjfo.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gyomolzpu.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/ggvkljhde.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/guyhjbjfo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gpbajrgjq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gjtwfikkz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gkghrewzu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gnhypxfve.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gzknzhran.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gbigrjbzf.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gmfgmdyjp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gxcofiyib.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/glqfutyec.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gohnxpclp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gtkbowotc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gljvgekgz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gmdjbpizj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gpkrzswtj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.zdbjq.cn/Article/details/gzjgijgok.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/genfwmdbm.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gnsrorwmu.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gyhbndhaf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gygasknsm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gtnosenmv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gzqvtejkv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/gshzbnhoz.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gryevlroa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.zdbjq.cn/Article/details/gcfnoevay.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gwgvrcdif.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gsseegmck.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gfthldtty.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gxsjuhsjf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gijrqtqgs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gpebgkobj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/gkrrtqzae.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gyzngzogj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/ganyuzkwu.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gwoffkhjp.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/grkryyocg.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gjmyzican.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/ghhxzegrn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gcloazete.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gprvlxvye.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/ghxytmgha.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gejiivfjc.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gjfbyvrda.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gvrfksoip.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/grmvljefx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gszpjkuyc.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/glvpfziym.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gukctvhmn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gyfnktnha.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/ggiczxxrv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gojypfdpn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gathntflb.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/grehhnhwa.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/gukxfucmh.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gelleftug.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzuugkhqi.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gggkohlkn.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gdqkrxkwr.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gvbqixjof.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ggnajvoso.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gyxkflkly.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gtotuapsh.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gbjqqkzsb.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gpmhchczp.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gbfirczxw.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gzjmbffhx.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gpdviqvkg.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gaymvamze.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gorrcuito.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gkktqehhu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyxkzyvva.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gobpziguw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyehucwon.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/geovyneip.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gwbnngqjd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gmcosoznc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gjgqtmpuz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqrolrjte.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcrppasax.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/ggojvkrfx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gnuyskdgs.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/giniefndl.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gwyadekzr.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/guepwnypw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gqxodnuyp.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gwihcyjdv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gnwbsuqqx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gnjfwfyjw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/ggllabeif.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gvmuvupkj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/guxobqfsi.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gtoomrsmo.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gemctyilf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/gzgajtvdy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/grlnlpyqh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gtaxlquji.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gzxcncbbp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gbxjuffkx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gauzkgyqf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gmqtgrkox.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gstmgttvm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gstlsesvd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/ghejqignp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gojvxaqsf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gyyenshla.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gjoamozpo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gccrwryre.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/geartthab.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gbqatmcdb.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gxkenlrzb.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gmsoqtbbu.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gktmuxouu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gmjllpmsw.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/glvsxgzwt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gigcmwxln.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gfknjjyew.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gbpjmygqf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gyrfelvuv.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gpewyrszk.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gfukwufqo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gngacbvni.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/guqrwausd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gqkcjbgwf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gzliewrtb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gipsipthb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gjmvvmbvh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gvbqgcntf.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gnbzqgtjl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gtcwozoht.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/ghmxdbekz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gixidkmmp.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gogabgqve.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gxpjgfjry.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/ghqsnnpqe.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/golqandeb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gxsgitmkn.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gklhujgjp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gdtgfydvb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gfeswwhna.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gbytsjitp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gjwlyjmtg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gedokckqy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gyvznmbvc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gvhzradnz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gilmwkozf.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gtzvwrmbv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gjplcwail.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gqskxvuwy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gdwqnlnkf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gbujsmdaf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gwllsmpif.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gqesgaexz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gongclufn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gukttxmlt.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gxygouniy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/ggcfqxvrz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqrasjm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gnrsmdjtq.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gqgprfgyo.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gfhuqryxg.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/ggpuueabw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gvwqmwmij.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gneqajodi.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gcqqfuxst.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gvxoionjz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gvzrtzhms.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gcgwuhgtw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gpfqaatst.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gmhiockkx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gxuawcbno.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gqzgcahxk.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gcapxvrdj.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gznslpanw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gqxobpltd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gdioabpna.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gbpkjetqp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gympvahcn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/ghzitamkv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gqacuahnb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gdgpyyeey.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gwdclilcj.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gwifnrvjy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gkxochasw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/grscxwkmp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gjwnexpvz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gusbgjmcv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsuyhuoqi.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gadhupodv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gktshqyfl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gcuowsiig.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/ggurudjez.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gfaisgueg.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gtaneeklm.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gxokhzhnm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gdogmzcag.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjucjlpx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gyuguqisr.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/grtkohwcb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/grsmmwehw.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gtlmykwav.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/glyvcziux.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gdxaahpfn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gmzgotgfs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/grguunojh.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gaqzdlpsf.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gbmsjtcvx.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gsgehaela.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/ggmpsyabb.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/glksixrjl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gvndfwdug.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/ggwrthalw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gbatzxfim.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gjelbdlgz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/ghhfvohcs.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gjrpmmxlj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gznbuaktn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/ggoemzndu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwddwqfrs.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gsticmrcm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gahnnwuvq.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/glveyhnde.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gzpqfchzd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gmrqzywso.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gxtpxrbyg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gymgfplkp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gqmmodabl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gboraaoga.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gnnngkdui.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gjtpdepjl.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gzlukxwik.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/goutriitk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gtvpawkvi.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gnsprzvni.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/ghsrunkch.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gvxjdmsqf.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gmldazxtu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gebolwngj.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcqtnrgmh.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gnnbfritr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/glriyrjqj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gvyapalbs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gxoqgpvjd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gxyvfvmsm.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gmfmhujcy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gompqacwo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gxpvzrhfo.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gfielgmoo.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/ghlgnuioy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gmfbiathb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjyyamtad.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gcclnrnts.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gxpgifilu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gkfmlsxda.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gxmafsise.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/goemsfptt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gefyssgae.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gnyomluhr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/getzcfpkl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdjuaksz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gssscmupf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/grdinbyyu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/geyjjjnhj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gnhwvirzz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gehbzbgtc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gokjvsxtb.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gvcqewyqm.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gvtazhbif.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdngzmaap.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gpnnnicje.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gmtbnhvsh.sHtML


<!-- 参考信息 -->