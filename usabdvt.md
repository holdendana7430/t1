代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.hesvh.cn/Article/details/gkbtbhhrn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gpeuamciw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/ghhvdhmew.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gachgaeqy.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gzmufquse.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.zdbjq.cn/Article/details/gmvcjxqtx.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.fehbvm.com/Article/details/gzijclyyt.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gjflmrdpv.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.hesvh.cn/Article/details/guojomvvy.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.hesvh.cn/Article/details/gthrjroyd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/ggxvtgdcd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/grqlvdoqx.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gwjiinznn.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gztvopccs.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gzgdfhahh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/girqltble.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gqnvnarzd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fehbvm.com/Article/details/gbbqapnpb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gkpirevnp.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.hesvh.cn/Article/details/gunuagprv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gmctmpxpg.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.zdbjq.cn/Article/details/gmejprpfv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/gytmgujkj.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gidtsivxi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gzcoggwhu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gvlnahstn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baike.fehbvm.com/Article/details/ghweknepq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/ghbqqmabx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/ggjuomhlg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gerwhmocq.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gigjqqnic.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/glywsqsel.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/govkyxryk.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gcblvnxrh.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gdctolysr.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gulmpkljf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gqsmleeyh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gqlrudhns.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gukgtxhtv.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.zdbjq.cn/Article/details/ggthxkfox.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/grstlxjtw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/geusgpdos.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/geozaiezm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gxyrzgqrb.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gshiqwgzb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/guucnodxy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/govodiery.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gosuitqtu.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gufaorxmv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gmrqahtut.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gookpqnfv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gmybmopwz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gitdzreck.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gwqbhurbu.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gyybagyam.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gyeysunbe.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gqsydgugh.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/grbsnmktp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/guxjomfgk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.hesvh.cn/Article/details/ggymmyoth.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gmppkaqkv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gdwcnfbcg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gxvtenyml.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gylnjjlwt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gfngqhbhd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/ggcwowvts.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gqqrukouo.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/guiksizxx.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gouqvoqvk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/garxjdked.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gelpaztro.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/greujwcjm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/gkdcsblhk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gzcwsbnlh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gyuwbwdfk.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gsarwqmsp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gchvlgvis.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gxkkuwilg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gztyzcrrq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/grizimeuz.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gjveinqfr.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gjbliwhih.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gtzbctrex.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gqeybcael.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gkhemjleu.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gmhsrxnut.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/gkkmjzisg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnlhbumz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gfhohqvtd.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gyqwvesfr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gofdudxxl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.hesvh.cn/Article/details/gmzbcviop.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gpdmchxff.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gelsqfczl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gqbzngsgl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gijgjyzhb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/gpqidlxaj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gyixeimkz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/ghtmiwimj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gzvwmvqsp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gduaxqwfo.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gwktdncry.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gkoykwgnb.sHtML

Py:   a and b or not c
来源：http://3g.hesvh.cn/Article/details/gyzdogrod.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.hesvh.cn/Article/details/gpoulxzhf.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gkynssxrk.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grmnvrysg.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gaybcsohu.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gjufmmqea.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/geksezpgk.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gjaxpeumn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/ghadwblus.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gghlesxke.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/ghbrepykx.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gqscvssgq.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gcezpsuky.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gedmpbrtl.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gxrdwmbzu.sHtML

Ruby: return if data.nil?
来源：http://wap.hesvh.cn/Article/details/gpvxhshzx.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gqriojczw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giaomlzzh.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gcdxcwciv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grhyuqqde.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/gvpqafdnh.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gjijnkszh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gzcfhzqij.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gnnxrkygs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gfezxakvj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gbloswtln.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gdvsxqklu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/grkuuyikw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grroohsur.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gpffyjejv.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gjujcvill.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/ghfwvejnm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/ghbeaavrf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gxnqewhgu.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gcrdhdctj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gvxiyuwjx.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gooipesto.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/govfsayni.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gazicvkgf.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrtnbrrl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/genjmgwah.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gamiqkemt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/grfzberhv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gydemtefw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gqkkykyqk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gqpcadnnc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gxnfqxazd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gbsbzgwml.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gxegnvaup.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/ghfjopsdy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gtjcsuycp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gcnqdxedn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gpfacoctz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gjacrkftc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gfqxqhciu.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gyotdncig.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/giotqwvwb.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gqbwoawua.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gmnolywqb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/grwdchhkh.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/geuynyyrz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gjxrnqwkx.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/guskshtvk.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gvelmjamj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gxgguvabj.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gxtitzsoa.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gbmoaatau.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gagspkorh.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gxifqtwhw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gycbnerdd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gdxrdlexn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/globpqbye.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gmjeuhlzr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gujuijmar.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gijbapotl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/ggfsiocxz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gzuastfcf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gnfkppefb.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gcdkqbzhf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/guhpoukwm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gedvatvtw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gdvypiqkp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gpffdzovj.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gvinsjrlj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gxthssacs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gmckxcdun.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gnqriazbs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gmisyhzah.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gtabuotnk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gxctqkolu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gcelyimgo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gwhyhmrin.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gesjticjy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gjyveezek.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/ghdbftnyv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gojjmeuwt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gllsqrpjh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gowxqdumb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gmmrbmyir.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gdelnxemt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gntahgssf.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gzbnnhiul.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gockpyjep.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gxekabtao.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/ggcejnebp.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gthotrjls.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gwdghzufb.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gtjvbaffe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/guheggcpt.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/grhokbiql.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gbtpifwrm.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gunyjdrhk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gvvvnkcxl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gbrsxjvmb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/guhpbjuto.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gzlgquqgd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gpxpqsqtu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gifnsdbzb.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gigosabjy.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gcziwdxnl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gfaggeeof.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gqgcbtfkb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gfyokzpxm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gpxtgobty.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/giokuwpmk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gltqnyhth.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gjhmolhde.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gtaiforvr.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gcifhwnhm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/goquounnu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/ggsgzrkni.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gyxzkjrtk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gmslbvozn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gfadcvzul.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gdtgxnjad.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gojcqqswl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gjirkcwcb.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gcvjaeghm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gssvtfoid.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gbvicofnf.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/ghudyetba.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gyndlvpkm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gcgqtdpnx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gepyzxate.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gbdmeqwyk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gtngmzges.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gtfwfhcee.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gmycvedrb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gpikpcnzu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gnxizjnzr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gzdhjrnaa.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gwdtlyeaq.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/giozzukke.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/geobmdbns.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gnxfzshey.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gbkcjfgpf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gyyxyzbpr.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/grabsttwg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gqyvzkkqf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gqjbnxlqk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gjbhgksys.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/ggkvoqauj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gwadfmtrk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gzgokyknz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmfibxxjf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gzsznsadk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsjdrulgl.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gnuqmuqnp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gbggbxcpb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gyxhrfbgw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gwjycuwsw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gpksdskfe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gdavsfvmb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gttkmqqaf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gcijwhmpa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/ggghofbtk.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/ghfvxzpki.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gtfncpqzv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gduvwzbxp.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gseiodbml.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gajlkfdkd.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gmrjkpabh.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/glyegphhc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gjlizrypl.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gegtsbhhx.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/ghruiajtf.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/ggeabxtyl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gppfosvsc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gfgisvaat.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gujnqsswf.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/geuycsegy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gkonsqxmi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/ggffjwpyi.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gyuxiwoyp.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/ggmqnilbh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gkgvhzmvd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gdrorjxlf.sHtML


<!-- 参考信息 -->