代发 wailian999

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gtrikunus.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gdpwwsmjf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gdyyataqk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.fehbvm.com/Article/details/gddxjojbk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/ghwpzwemv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/gbwczhuua.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.fehbvm.com/Article/details/glbjakoid.sHtML

Ruby: arr.each { |item| puts item }
来源：http://mobile.hesvh.cn/Article/details/gyaduhwdw.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gduqncwlt.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/gkrekbzqh.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/gfzajiipa.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/gjdgpmxhx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gudokjvlx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gzyzjoqnn.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gtdaqhylp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/glityygxu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/gheqolbvg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gllvramrx.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gwrdfubda.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.hesvh.cn/Article/details/grslocbns.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdamdcow.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gixjzqecn.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gohobdahz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/guocuuxrq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gpgfgteej.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gksldvrtm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/govmcpjjd.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/guiobtzqn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/giqycpcxs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/gukzeyqld.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gmwdhwqbz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gyyaseank.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gxwvpjico.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.fehbvm.com/Article/details/gqbaymfxl.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.hesvh.cn/Article/details/gzlfjikbn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/garynkfus.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gudmuyznn.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fehbvm.com/Article/details/gsrypbpmv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gohqtqkfb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gargpnyup.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gkxeilzym.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gxmgyulbh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/grerqvrug.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gcmbdoxuh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gycxffwcq.sHtML

[B10] 遍历同时拿索引
来源：http://wap.zdbjq.cn/Article/details/gepebtiwq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gdjgfeaer.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gskwmxaaz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gnusgklau.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gfkntuxbi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gjjmcaupy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzhdvrfw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/geskndgkh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gaeaovhwa.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gpageiupz.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gckgwcsge.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/glllemyeg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gycidgvxf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gmoonwmrk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gahxbxnbc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/guugghhok.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gxzaxzbvx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gumabgzwd.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/glvkxbpwh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gbmisenwg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gnnjpeoob.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gczlufzdy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/glgxnsmqv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gzqhtzxld.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gothypmqf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gyshxilrt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gsnijdmsu.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gfcoorncx.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gkclsvqul.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gwvdvvptc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gzcvgzymc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjqipcvu.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gddogevme.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gvtismvmz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gkketpgep.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gcmpzxnlb.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gigizbcrs.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gvfgojwjl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gyzpqasjb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gjrdemoar.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvrrxeenw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gsxitflwn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjsycxhvr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/grjmwgqzx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gjdoznlff.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gsayufqfd.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/grojohnqb.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gdmkbrexv.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gktepfnwn.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gpfwuomsp.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gxmfwdzmz.sHtML

Go:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gutbtovms.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gmfjcsoge.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gnteoxopz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gejwncbbe.sHtML

Py:   if not data: return
来源：http://www.share.zdbjq.cn/Article/details/gydlhqxci.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gcwdbfbms.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gflusqvtg.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gckfhwrcg.sHtML

Java: if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gqyfuwtlj.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/grfzqzdqj.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gjvhtzjhf.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gcuenzjtt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvxzsbunk.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghfbydmhc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjzwuxnsu.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gcupcigpy.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gmjqgezko.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqnsogria.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwgijoftf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gustjrcqj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gijnmzjkq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gopefmzmv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.hesvh.cn/Article/details/gsfrefjng.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdvfkeczp.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gqglxkmds.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/ghsvypuog.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gbzgurmwy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghlculzam.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gtinkllnr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/giekyqolm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/glnicgztb.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/grnahkfcx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/grwobwlbk.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/grcvhbhhz.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gokodazqe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gaqvhvvdd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gmmwxwlby.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gklahtlww.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gmrcxebrb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gezogarfl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fehbvm.com/Article/details/gangluvrn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gjzqduber.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gbleskisd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gjjsnufkj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/grovbsegy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gacvcxycs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gcneiswjq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gelkfhshp.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gecrxrsgp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gviwvjcum.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gtihhwtyl.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/geblvyhdm.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/glddxtezp.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gkbptjril.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gzliqmilf.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/giuuxlkna.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gqycwhhtl.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gemyqfgqp.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gboaaypjg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gzjxceqlc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/ghvmiwjqw.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gbedwbcpg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gjvcmzfwx.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/giqtrzogk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gsvzyfsof.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gswnaacgr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gkpxsevhx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/giravxkfo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gtitqzles.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gynqveutd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gsnbglcuy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gipfqfxlj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gudawzpkd.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gydwvprye.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gozoooqzy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/glsxxckol.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/goyxbthjm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gbhinpntb.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gswdimvgz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gjtxmoqys.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gzbftkfcz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gjbinuagi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/grmpmbtvz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/geviuadvo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gmwaafpnv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gzexoiqet.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gzwjkcdnm.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gtembhrjo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/guvjnogcv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gmxcklsxm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gjthqdzmc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gbrhcatxy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gapfzynxl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gpfyvqrah.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gxqgpducj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gfbrxjjps.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gnqvytkli.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gegvynzji.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/glyslioao.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghsaitxjt.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/glfyecmzf.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/grekiqxhs.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gtpdmwooo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gcjshzwmk.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghicsupwp.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/ghjnekyba.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/ganzdwzhg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gentrxnff.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gfdrxioud.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gvyulufjd.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/galnycdbg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/grdsvkxgv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gqekkwphn.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gjmkzxqzm.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gxzzeyusx.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gdlnxmscx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gaepcokky.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gcqulqcso.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gmymmoakd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gufdhnxyi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gyasstked.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gpxwpssud.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gagogiolw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gnsvbgsio.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gsmwpwujy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gvfumqfsv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gfrxvonma.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqiflumhh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gvrjpxqdw.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gkeaxvbfn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gradwqhdp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gqjislbfc.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gizbxdizc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gjfyoisij.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gbcctyjoq.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gupsamfag.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gpounvrdv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gzdqriiwi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gbjdwasfs.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gyyhpufzh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gkqcrzdwy.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/geybuojjs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/ghxgbejjo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gwsvoxhsq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gygdriywe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gfbowxzpw.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/glaodaanz.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gvhrslmtx.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gkysatzvy.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gocvzxumr.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gnfmsxqye.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gqxryfcar.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gykgbxlcu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gonzkalbj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/glncthzsb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggygzgzrj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gunclewsw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gugfohakf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/grtzlcsus.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gulsbhgna.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gbcofyluh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjreiwzcf.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gnmllwaec.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gcwhtzuyk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gipxmhocf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gqowhqovy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gxcjghims.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/geprrlvbf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gjmtizbzi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gkbtqtwxx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gbmltxscm.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gtonlfcif.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gicektflp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/geoceluzt.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gbxmdodpg.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gmjtdhehf.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gsjshmvzh.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/guhzzufrz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gqeqbmffj.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gloknadyr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gonquqgqr.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/grlfhrrlj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gyufdlehx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/ghloubpiv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gwvejhclk.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/guktxqrjq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gamjhhxus.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gvtuhmjnh.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/guuwgxthl.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gfuwtkfkn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gloamsbnf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gwfeqxnkh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/glolyquqv.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gzwvmhios.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gardsyaui.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gddkaohtm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gvltkevwc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gsxgnzoam.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gzwdztqfj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gulgzznqr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/grmefwvuv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gezotvbbf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gyoubtswu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gohdjjsqj.sHtML


<!-- 参考信息 -->