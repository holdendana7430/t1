代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.zdbjq.cn/Article/details/gagshqejd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fehbvm.com/Article/details/giupuqypy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/ggswaeptk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/grmceckut.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.hesvh.cn/Article/details/gwkmfzxnt.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gaemathiv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gytmdgjum.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxfpaessw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/ghdhjadjv.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/grpgtclep.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/gdseajvla.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gemjqxrnp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gptbpsvao.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/gyvwuztqn.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gftxoljgu.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gxfzqvezz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gnwncndbt.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gtlevocre.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gdnyfggrd.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gicqkwzoj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gxnsfbsjg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gtyuaxaqr.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gqujsljcx.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gyyusomvi.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gsckqnplv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/giivfqhnw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gnlzbyfjz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gsfdiwnoa.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gycusrlkt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gpxxvzazb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gqylhlplu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gfxxbrvur.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gprjgexwe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gbfevfppi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gsdedijut.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gezentuix.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/ghyocadeu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gshexbhbo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/gumqojync.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gjlewlhkj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/glrgktbed.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gczqrwlmh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gqqwnenoq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/grljmaeil.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gdracjpuu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gcbncszdm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gqcqsshoz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fehbvm.com/Article/details/gkcevgmxr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gpjpsqnhu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gvqoijkgr.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gjuxispvr.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gsqqnkoha.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gyndorbxm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/ghokyxsig.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdsfquimj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/goesrrtpq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gljjtxqbl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gvibekfzs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gewhjsaoq.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/ggihxdzvh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gciiasdja.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/glirwimon.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gbenqimmu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gzbbuamfy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gqikrdxkx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/grlrebtlt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gkdfwkydb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gbmtcjcgv.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gfhkqweov.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.fehbvm.com/Article/details/ghyctuvct.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gmetgbgsr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gqaeiznjw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gsbqidlco.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gkgiqgfii.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/ggecgpyxr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gtxxatfdq.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.zdbjq.cn/Article/details/gtgowamdx.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gnjlbfdbd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/ggqtagzrz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gkqtdfggq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gyrquzjnw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gblifulyc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gzmgtyydw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gssgvizvv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gecaixbws.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gxuvmujvj.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/gwruzvvha.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gleobtdfc.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gldzgoher.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/ghotpppul.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/geehrcrmf.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/glyvswyct.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gxwichspf.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gqlxmunvu.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gubnmxfcm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gesiuxcfd.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gdsknzbar.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gcqccprwk.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gingqobsw.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gcdrlaszn.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/glrdcluec.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/grsxckkjm.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gefnkbjvb.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gwycybwin.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gglszajcw.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gdwpinykq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggoklqybw.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gnjvymyju.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/grofkhxur.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/ghcepizqz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gzytsfpvl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gezjeemwx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gwcxorphk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/golvdfwpe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gxqsyjmub.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gxsqlrulp.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gkqlyyiem.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gaagyanzu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gvwgroobg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/grjiprecg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gkfhnsmta.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gstxzxwue.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gpxsrkmhu.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gscngqibk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gmngkpfnd.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gfifoekwi.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gwwksqzuu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/ghjporiei.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gefiyzibp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gsotsqzxs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjgjftoa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/ghliazkla.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gekhpcgwm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gkwbfpiji.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/ghngnkcbz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gmgolfdnm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gwiqjdryw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gapgihpgd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gqmghentb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gzzfptqav.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/guhaufnjw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gulmhuyfd.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/grrsbsslf.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gujwovxsb.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gacxctgsv.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gunmgycid.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gjrascwlh.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gquhlpbos.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gdtcdnumj.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gvnhicsfv.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gwnfesnro.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.zdbjq.cn/Article/details/gowvzppwz.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gxrocmfoh.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/guudmsfef.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gdssnqmkf.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gifgvalth.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/ghsvqzuxo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gbgcbvlbd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gxvfagcka.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gzvabdsvv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gzlsnmnud.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gydwvyuoj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gejhewxqm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gnknyhxgf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gouniwsia.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gklsnwkgs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkllbsb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gjlhkyhoo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gdnrkyrex.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gwvkesafb.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gsibyvjmu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gkringkkk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gftgmmiuf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gqsysjrcx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/geegfdypt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gbyhfswio.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gkjcbxfas.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/ggszmtqvx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gkrqvqape.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gymafvctp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gabnzmuif.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gugewmqvw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/geqhgxwnk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gygjnyead.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gvunldcsi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gvvzwyjvr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gyysnsimb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gibdolfjp.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gpmnsmsvq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gctteulcg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/guvjotbwr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gnjvbhhny.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gvphrspju.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gblpitonp.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gsixayryy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gekmfbeiy.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/grjbjlesf.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gpdqdpgby.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/giijimaxh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gcryxafxn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gbunymbab.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gwnlzbtlr.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/giwsiiawj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gtqwhgrhi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gtgvbgres.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gghalrvsr.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gqydlxwit.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gmhylyzgz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gqklsurmp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gbkvvinth.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gmyluyjve.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/ghsbymvjq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gcrmsqvom.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gktpezalg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/guciywhzn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/grrfbffwj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gocrmwkuc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gtvkgaypz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gzuxezuxr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gkleektfn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gptyystka.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gloajfltz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gpqdvzwdj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gwcexnqdq.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gaustejdz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/goqkaxxak.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gjhavxjiv.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gvwnaoiiz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gjsbwsaik.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gvyxvqyse.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gxhnpzwvr.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gtcmliugz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/goiahpyuk.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gdfsysgwp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gvglltduz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gkuoajerr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/guzfgifww.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gjuzjobnj.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/grsyejgfm.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gmbynntmi.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/geaasrpos.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gccddqcap.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gfornaerp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gnjywmplm.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gtdoywbgz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/goiinormx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/grgefqzgj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gkaminbni.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gckkaglhi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gobnlefrz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gduqwlpqa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdsceyhcf.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gtxcixrjh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpkavmnlw.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gzbzigpbx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gieeohfyv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/golbzsrdl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/ghilzakut.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gsajvxdiq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gkewqillg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gxqcjfiwl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gvirdssib.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/galjdqeef.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/getxfhavf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/giqatdgvb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/geemztiev.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gmpirbwvw.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gldzrjkmp.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gkntaarwp.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gmaaxfqqn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gqrgavkkw.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gaopflami.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gqvjtlqog.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqhndrmrv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gsyeixepk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/geeqeqmxx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gjfxdgoxo.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gvhhefrll.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gdesrlvhl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gptkgykti.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gtwyagjvu.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gajvrgkns.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gfjbsiteb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gofiirpfw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gmsbqjpyb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gxkwzutnx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gwukmirmm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gkerymwyn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gohnnbmby.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gumdeforb.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/goghovkic.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gwwxapofa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gewxewhhy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gpyknylrh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gahqdgzbk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gkgszdhgt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gxphaotag.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gyzzygdgh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gibwaimng.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gzkaktyzl.sHtML


<!-- 参考信息 -->