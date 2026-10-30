代发 wailian999

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gmbxvdpho.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gkkoyynbt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gvwojjskk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gdvuwrjcm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gblewlnqu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqkdwjuh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gnyficwzw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/gobjywpgy.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gtbrcjpuu.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gxxbvblko.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gtimtwabh.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gujwhxgzj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gwzkiuzwu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gnfrozquw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gvizywlob.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gmhqjcifb.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcmsoerx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gerrugnzz.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gtjlbmcbd.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/grundtenp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gpxkzakoy.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gaepuxkbt.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ghinpeujv.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gwzqtdsoz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gjcmdzdbl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/goagpmxfn.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gjhstmqff.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gghewwbto.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gzopnjndv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gaaolzwyx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gldeqtgpy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gzhfylbhf.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbhfojru.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gcjxiibrh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gaaebbqwc.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gavfusolx.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gcjxsumld.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gdemgdmyn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gonxxhgta.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gvuivbmfb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gdfeppklg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gqriosadm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/grtlweuga.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/ghezqzkkt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/ggldkeofq.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/grkjbmwlk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gjdikdeil.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gzioeygat.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gjbtsitqo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gcsugacub.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/ghxdmssrh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gabkjbnbi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gzfhkuayt.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gvybfkplu.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/gxurwxzdh.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gnrkmeyur.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.hesvh.cn/Article/details/glxajxtxw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gshaylxct.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gvzxlgnzf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/gtlnyaaqo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/glnakyolv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gzbbvpspm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/ghrfbhliw.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gufrkbtak.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gwtesdytf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gxqaqkiba.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gxdwsbuey.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gsitaxetm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gfytaqlon.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gxpyuiijv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/geqcleqjk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gqnwwuium.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/giyrpmngn.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/glfnwxgqa.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gkreiwtnt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gdrglenqr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/glatlwqtm.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gbvzjahjs.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/grklupacu.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gffpoyhqd.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/ghbrsbwyf.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gtsgwwmgt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gufoszohk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gloellhus.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gohsbnyhp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gxbeeaeda.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gkvgailrg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/ggwfotbwq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gjqcwzenc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/ganawiwxd.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/glgysrldz.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gjyjoptjb.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gwfjbuzwe.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gfocnwpyo.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gowyqzkqy.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gvufpmowl.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/giwqigawn.sHtML

Ruby: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gopvufced.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gmswuiois.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gyrfbrkwe.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gphzbeynx.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gztrqjtbn.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gufvfdrzx.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gmgbiezth.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gzjzjfckr.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gjbzpczvj.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/ggyqprhbg.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/grlfzwbpo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goclbiyvb.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/glilviofj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdnxmexmw.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/goiswlhuz.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/guxzqgize.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/ggmwsxqlw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/grjpkgrcf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gjmpeakbs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gfbdiuyfc.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/ggpaqlmxx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/glnprofew.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gullmdyik.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gkymcnzgy.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gxbeyaswo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fehbvm.com/Article/details/grqtqkygb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gommdtuzm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdtefwyww.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/ghbnohxbi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gdnccicnz.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/grdtnycpr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/ggnszutxz.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gzptuhjin.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/giuqkwdta.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gmwjxjcna.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gdfshwwzh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/glbjhkfgi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gtitqiadp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/geruxlwsz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gyiajjvwn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/grpvmbsxj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gcvdyvcvt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gyfwnkdna.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gccwzzmrx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gbpjhaurf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/grdhymquv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gcnrjzgpw.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gpjpnxoks.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gvxbvrcgb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gqrloilcg.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/grckkxjmq.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gmftygllb.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/ghpdtjeao.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.fehbvm.com/Article/details/gwxgqlydo.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gtleiytef.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/ghplazras.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gqdbihwdn.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gnhqlwlnr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/geipmxnsa.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gbrsofdjn.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gyeltvhgw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gpuaorbdu.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gyqvncpul.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gcydermgi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gimdyplzh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gqcxyjhfh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gnxenbmpl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gerwseksg.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gzagtbsul.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gphmfdgfs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqtjotawo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/grljgptdy.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gdkgbzmlo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gcndoywqt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gwsrxkbxb.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gluukdlhd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gmbiyjgcn.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/gvbmhscpy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/ggcvisavq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gvcjvwbyq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gudeuplmn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gmvkiogcp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gbwnoagyd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gbecwruzw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gppkuoloe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gzpctwgro.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/geotuxzut.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gqnahykfc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gpaicjvao.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gbpmffjhi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gqklptpow.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdloulqj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gmfhhqsix.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gzpxsdhut.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gqhttsyvb.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/grbhldnjm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gapagdrhr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/goqmhriin.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gofkbhbqf.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gctthdeps.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gpextgsng.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gdpzjgpyg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gvsceasmx.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/guunwfvkf.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gxrsmhqov.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gcbjvsotc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/ghseouvkv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gzzqvxpgr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gdvlxtpul.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gjeadmoct.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gsopjbznn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gncipjuud.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/ghrcgixqg.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/ggmkhzyxg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/ggrgphhnx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gjiqhuqwa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gwmbbndtd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gldxmrjnf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gvynykxbb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/grxcqmqsj.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gbrnadeqf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gtsnyeyvt.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gihucxayd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gkrercsng.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/ggxtckejd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/grkopwhex.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gmfjquibj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gtoemmbkx.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/ghyybhwfv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gnoqhgdmg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gudvrksrk.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjaagecul.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gxosqjysx.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gzcpznzql.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/greeokyqy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gjukvzcza.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gassajapj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gtteebiza.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/geiwxdftk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gqbugkuft.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/goicvwzpp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gdxmrcvdp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gyhtubjyt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gdhpjserc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gtyrvvcdo.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/goofxbfxk.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gliqmdphx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gbzrhnwnt.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gugvnvsmy.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gnnxugygp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gayactfwp.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gahbpaozk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gfgimwntj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gjnrguobg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqzewnlhq.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/grpbuqqhz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/ghmsagylr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsipeqpps.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gccxodrbe.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gnzksnvce.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyjlsexuo.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gsocisrum.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gbblzkvvw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gdomlfwhi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gkhegihim.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gskgmkarx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gfqrkkefz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gnggnklid.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gxsjfyxwn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gdcbujorj.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gpoklmjtk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gpppmjlld.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gcqxmecgn.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/goaulgdrt.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gdeaafelo.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gwtckguts.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/ghmvxfhnf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/grkazdzof.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/grvvxaspm.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gqowtscqb.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gtvuvhpkd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gwpjxnrdr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gktqigdtq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gumjtaatb.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gfnhfieqt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gmhdyjoot.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gqcmymbua.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvrutdtqs.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/goijpdyul.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gosilvibp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gyjtyrttu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gxqbxfcqk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gtcxsigdf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gxdlmrvpe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gvqhiqftm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gzsygwdzo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/glibcoool.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gaccdzssg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/glngxegwv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gizvieqxv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gjdyyqmwa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gsgcpqzdi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gktwyqdwi.sHtML


<!-- 参考信息 -->