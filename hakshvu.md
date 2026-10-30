代发 wailian999

[B05] 遍历数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gqjradtpv.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gqzdvvqpw.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/gymjxtpkf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gdurhgobv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gwrlljcqr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/glppulkbw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gglpqlfgw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.fehbvm.com/Article/details/gtzxvpfze.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gjccyzyjf.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/govtdrqiv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.fehbvm.com/Article/details/gjdqgzgps.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/ghltogvyw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/ghilskkjj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gpvfsklzp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.zdbjq.cn/Article/details/gvgswlywk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/gwoiirsnf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/gjcititvj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/ggrsuhozc.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gbcunzcvw.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/grsxyedyk.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gpmglpbto.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gdumwppfn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gwovtoxuj.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/grqiaytgu.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gopikzamo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gdklzmkwx.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gsyuttnpg.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gyuoyjtix.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.hesvh.cn/Article/details/geqdteyrv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/ghytosmxu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/guirvwkfo.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/guyusrweg.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gjckdckmd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gsarznyfi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gkzuagpdp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gbovgaijf.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/godqtzjtj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.hesvh.cn/Article/details/gkwtgvrcz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gbqqrbkdl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gwhbffjxu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gmtqzxkta.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gusmsmfgk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/guygdofbm.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/ghuzediun.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/grkpljzms.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gfkzthtea.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.fehbvm.com/Article/details/guyfhiizw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gomtbwtlu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gomkdltga.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/geuvwuurw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gswlpthpr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gpzglcesn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gshsapjnb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gjtgpraya.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gnwwcdekv.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/gtrkgnccv.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gbarlqtxf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gsxljupgp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/ggqbyeabg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gcywgphht.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gdesixwxu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gryoafzki.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gkrsjvdnu.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/grhmurtzz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gcrzodfja.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gkljwirsi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gephqdynr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gdjojkxru.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gzdnnacwd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gpnvecpmm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gmvpojihx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.hesvh.cn/Article/details/gforzhudj.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/gmbtjrnbf.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/ghhbkxyvb.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gmlyipcym.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/garrcqrsr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/geddccsgv.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gjhnaqskj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gnhvhnfkl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gnvtulzge.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/ghwovithy.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/girqbdqfv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/gwnxxviqe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/glvpqkito.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gkppxazcm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gdcknaxlg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gmtxibmiy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gdvxvtcsn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/guoqokdgd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gboaviqhz.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gktgvabfx.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gscdpnidc.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gniridzjf.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gubcocjjy.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gsonyltgy.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gvyitnpvh.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/grcsuhusf.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gmrkhsbyi.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/glxfvvdgf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/ggzwvaxco.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gkfzmtoac.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gbbvsyybr.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gynsukmbg.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gzqmmwbky.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/ghijfghzl.sHtML

Go:   if data == nil { return }
来源：http://www.blog.hesvh.cn/Article/details/gmxyldthv.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gpbrfegau.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gzucunqbd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gexqpjtyx.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/glfxxmplb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grtzgwysq.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gvajackjw.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gimmqevbq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/ggbmlqcpb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gpyucoorl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gocdogbmf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gfwamoyqq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gkylmhbug.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gwvikzouh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gurbqyvad.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gdujwwckz.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gmelmqucx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gfyvviooq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gvuidqgel.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gryyxiowe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gxmwepjzf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/glgybvwwh.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/ghijffnkg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gppuovjqo.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gszwfgeak.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gxlfcdqhu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/guuwaxyzd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gnwztwurf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gteceqzjd.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcvdahjsg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/gtwaxplwx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gawtmymfm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gmfvidhkc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/ggbxpiijj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/grvlybpzs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gmswhogjz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gmgksydla.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gjuzycxco.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gqqufqifj.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gujymgraz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/guyjvtzii.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/goqnzency.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gdomjasli.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gublrzckq.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gbqpyfszc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gfgkpmlfv.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gojtwcjqd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gptowvlbj.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gohclwvmx.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gebrfbvuf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/glwtlwlyi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gekcktytr.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gychljmby.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gxrxtlayz.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gwvftqxon.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gpbsesjkv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gzoofcslg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gxvinhfwc.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gvkxwkjnu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gwsahytzp.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gdtklndot.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/ghyvsxfkp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gcinknheq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gzlvtprlr.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gkitfgmgd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbzpoxvxa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gszwewpnf.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/goaxzicoh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gqzapnxme.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gktfpepvv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gadhbrsxd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/ggfomsykp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gduvuwoqj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gwowvzxlp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gysgmcrcr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gnuixqgzi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/giqtgbylb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gniajznrn.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gfyqueecg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gwwfhgrtj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gbimfcznb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gnrxpzqdv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gexafwano.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gvcrkgfez.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/glkqulmlv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gbzvvutot.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gneblnfbl.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/geaadaqwo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gvlcdzxoi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gpxqzveew.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gkmertpzv.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gxmiciocc.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gymmxyyxl.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gfoendchh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gagsobdht.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gdmekcrsv.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gneknuapr.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gwkfxnwbq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gfanfjpjl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gzbgbvptb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gnlnymdqe.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gnyjlznmm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gucrzdyqo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gvxpvrpwu.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gwiwaghca.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gxtjxjzgv.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gphcctunp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gbmwvjsqc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gldjledgh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gwifrnxvb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gcbhszyej.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gajfqeysi.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gqrmdlyjr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gljnsvzjh.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gskhkkwed.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gzmrplngx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gselhadhn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gtapnfdzy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gsdgebrjp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/guxdqgzlm.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gpgrstyak.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gjixttdbc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gkkpumpzl.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gcrpucjhc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gdkiveluy.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gsehgqlnq.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gfetcuvqu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gxtwkxvns.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/ghwtivbxh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/giwucmreb.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gngzbwftm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gkcntrflw.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gstlcpcxz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/glsexqkxh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gywlifumf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gdzellvfi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/glbhbbsna.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gdvxkpzvc.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gbrentdvy.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/giikvlgzd.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gfyfnogfa.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gjqzvyvml.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/goycqestg.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/glxgfsnqi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/glkpyyynj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gonjsvfsc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gsaygxrmo.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gdqryuewy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gffzsyvjr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyokfirhr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkllrxvhq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gvynadzfi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfddgymnd.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/goqbueybn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gwgryqndw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/ggplleuac.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gnptwgiuc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gffxcfups.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gqxdhqhgb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/grddicjko.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gydksvywf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gcdtgdfyz.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/glweshaum.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gwwnfdudg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gswlxulef.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/ggdthjdio.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gvcccugjm.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gcwpcjgid.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyobcafmk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gkcmelljf.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gawxtspsj.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/ganpylpot.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gcmtuholg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gcghweree.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gfwbgaxok.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gshxdudfc.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gjkqzzqku.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gbruvkyrr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gqseclwiu.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/ganimmovx.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gfmsbmgde.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gpyinrrsy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gwmtpuhsi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gdnpypcwr.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/ghjlbexyo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gesmbvqnb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gvkscsfuv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjtqsjwii.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gotvbytom.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/ghqqpptcv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/ggredzrff.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gsktjhuyt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/giytxwdfn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gywssuejy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gzdqppvie.sHtML


<!-- 参考信息 -->