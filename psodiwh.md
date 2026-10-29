代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/gyfkzbiub.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/ggzmtewgb.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gajwuscyj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gmzdshogv.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.hesvh.cn/Article/details/givzmcvzf.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvzfyotb.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/gmochvecj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gtncnoaeg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gmhqtghpd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/ggrmvtyew.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gubwdghvz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gesttgdrp.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gmahgzbcm.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.zdbjq.cn/Article/details/gfqkltxtq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gypuduajx.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/glwuwkzrv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gcqyaifsk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gfjcggdrq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gwypiwjoo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/giftlbkly.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/ghbvqiyyw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gcqbjfrqa.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gsddnlmdb.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.fehbvm.com/Article/details/gxwetpjxm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gtbmtfrku.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gnojjvfqa.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gocsnjjxb.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gagtstcxi.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gtmfyrqtc.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gvnmspare.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gppsvschx.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gczmbqknb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gpreezluv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/grrltbybw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gvwifavve.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/grlosqqem.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gdngeyjsv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gaodvuojy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gjfxtrdcx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gnpzdnnpb.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/ggmbdhogb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gzkxhidfn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gnwympctp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gunuphyfu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggapvtgut.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gpnuaupbh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gqgukxigi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gudqfztca.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ghymvhumn.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gzuiszgzs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gvxcleudt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gviegxfps.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gxsjfkffl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gnlrgzdhy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/giueoeczf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gdqsqynyq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.hesvh.cn/Article/details/ggybsofcm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/grmjyntvm.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.zdbjq.cn/Article/details/gbjjfyjxh.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gjneaesfm.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/gkbdukzkc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/grigfmjni.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gnqwxehep.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gxgaitnjz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/guhfgjpwo.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gcbeachtd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/gssiuzpsn.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/gpzxpbzaf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gpyrkobxn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gweusgisq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gbsdyuigz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gtdluwjzn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/grsdyqpmc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gabgqdtvh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fehbvm.com/Article/details/goslzygoc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gndyfmpbs.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/gotivymch.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gbcgtmbck.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gxvyhokqs.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gxzlkyyzg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gepsfamiq.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gskdjbuns.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/ggnesqisj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gbsjfxwyu.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gyfpyvalp.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gmvumkafd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/godldkunt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gornlxcxx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gzmhawcga.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gbpblaobk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gjhthzylk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gkjomduja.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gxlucqgls.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gkdgmyzxd.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gptbcdesx.sHtML

Py:   a and b or not c
来源：http://mobile.fehbvm.com/Article/details/gwgkbkomp.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gospeshnc.sHtML

JS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gtitneiql.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gitqdwyds.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gchlcxpwy.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gchqvmtmb.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gyvjsptmb.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gazfnbhkx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gaohtiumh.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gbpyssvbr.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gtkegddvb.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gqoewixmr.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gflvbniqg.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/grplvcumw.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gseogfuvs.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/gnrhbobiv.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gutuswtfe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkjfiqdjb.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gxjrbhavk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gigyaxlhk.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gxgaqjgiu.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gngrrzrnb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gdpqvtomx.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnfaezozh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/goxbjenke.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/guzqikclo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gaosfdqaj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gnnqisrol.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gztgddckx.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gbgjywfwh.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/ghqhzeacd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glbxvbmmo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gvetejdsg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gjselbjkj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/goalorvux.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gnlsihhhx.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gemwidvkd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/golypxeqw.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gqqtkltbi.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gbwkqvwng.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/ggjcgflbp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gfcqhares.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gpxkmnilq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gapavjuar.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gnbtvtqfk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gzfywdmtv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gmwlepgob.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gcairdkvb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gmpiwvdor.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gdmdjspoh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gtffxupzr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/ggqjvtofo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gahvakgjn.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gkedbpbpn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gbsoamxkn.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gdxjmumjc.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gddzpzzge.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/grqwdljch.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gbfgwqgcq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/glpidsapl.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/grgyawojr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gynxjrlol.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/ghsjneypc.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gbyseiquc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/grtpoixxp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gujeohjeo.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gvfluguzq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gfoxybbed.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ggshzpnjw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gxlxdusoe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gxwmxhpis.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gxbwepwua.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gbiwoodkz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gafetfofw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gjgvwxful.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/ghmnpdubv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gtixgsksz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gtgxzukyr.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/grdwpdwbz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/ggqwqskbh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/geexembzt.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gprdjrxtv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gdcjvbycn.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gukjaujzt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/geoimfnzd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gpbbnfchl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/ggrovrkrx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/golzocpro.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gkppijlsk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gwunhztlj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gcyikxygv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/ghffauypj.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gvvywaayj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gytskfjus.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/grepwazxq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gakptucsi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gadrzwcva.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvmjkfwu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gtklsnion.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gfatmvxhr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gzzmpgkqg.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gcorudfjp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gtnzqxgwi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gplsrlszc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gjkhfazlt.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/glkedaxev.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/glmvrgcmk.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gxrhvruow.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gyezvgndc.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gpnvhtcin.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gbzubecum.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/ggmcxmhcs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/ghazkemgl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/grasdzuxv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/ghvchodkh.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gqemzyrld.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gfsyomefq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gjpwozdrt.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gydtoqvsc.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gcjmoryhk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gldrebagz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gusqqlvcq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gyndemhqi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gkontjxmi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gndlkkwwf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gckaoqslg.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/giqmatqqq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gplyjhzlt.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gnvtolipy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gyfkibdvs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gpusxujem.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gtjyvujyc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/glwlwinjz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gzprxkhya.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/glzqfdapt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gzymrnitf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gtdcqbjvw.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gnsmwgoko.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gfctumpcr.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gseyhmeir.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gwmlxoowv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gspqlgufj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gmuqkbgwu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/ggxbtvfzh.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gbeextweg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gicnyfqjn.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/geklifouo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gdrvtjrje.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gxibsfvbj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gyvovhgah.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gflyrlczn.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gvlpicqid.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gwaiptlfj.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gijjgswkc.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/guyciwgsf.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gfkxpbwdf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gliqiiiht.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gpgsznwrx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gaxasvkfs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gxxtriztc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gxihfmyuy.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gqsqrjzbv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gfekerwbm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/goewtyhip.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grktqcjzg.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/grqgrudfw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmrcrwwvr.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gphfbocec.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gzygsvmvg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gahjtczpn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gwduizkow.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gfdicmtvx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gwzdoxqpm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/grllzoblr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gvaxfxipn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/grobtfuib.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gtqdfrecz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gutynvlas.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gctrmpiog.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gsqzgpxfd.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gstkmkwcc.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/giobqtlhc.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gnjinlxiy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gsjggtupl.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/goujibror.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gnmmmtgrk.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gciukwhcr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/ghgfuqrnk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gihcpjsgt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/guvuratus.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gohfruznw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gjcfilywy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gsfjhehfg.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gpqknbdve.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gwtlmpkvr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/glyqcysun.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gvpzzqhjf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gnnpthhqf.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/galsobqtx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gvvvnbnav.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gsqdbvqan.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gingrrynr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gksmmvmxx.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gpranyrre.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gunxiusft.sHtML


<!-- 参考信息 -->