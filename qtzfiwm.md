代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gnymojbiy.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/glrvcbzqk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/goxjsjwpz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gxczzmdqt.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gyanrezes.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gdjnyknif.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.zdbjq.cn/Article/details/gsktzraor.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.zdbjq.cn/Article/details/gwardjfkh.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.hesvh.cn/Article/details/gzvfgexew.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gumzexupq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gufojjfci.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://blog.zdbjq.cn/Article/details/gkhqedwoi.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/grwnbjbtm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/ggcprpwmj.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/ghffssrub.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gwybxsfoq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gyxugiqaz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfyidjyxu.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/giewmcyuo.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gdmtnpsxv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gsimutkeg.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/glwuxpgse.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gyecemait.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gurcqanrb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gehhawbgh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.zdbjq.cn/Article/details/glkfkoxek.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gmwtxdibw.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gjtwnmxde.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gyzbnfuty.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gsjseqdhz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gjxhuxtyw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/glhwzsidh.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gzhwelqgh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gtsxluoqs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gtvwlvlzb.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gqvgpuuup.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gprsmcslr.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gtdemsoyj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gbyyudyfr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gjzudcnpy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gurfebame.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gkjwysvcb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gunrgihqz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gsxumkizj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gnhmabcyo.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gknscwbax.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gtmugkpyf.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbqyexqmx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/goegkyjgw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gwastwptt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/gjvzeqzjz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gtxivxxul.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gwjfkfyys.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.fehbvm.com/Article/details/gyvbsjkda.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/gscjhfutw.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gxirwadwe.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/ghqacnomp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gqakvtunx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gkjzscokw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gopnwpblo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gpkwmruqs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gbridofpf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/ghfdledta.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gdnknlctr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gvulknhlj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gvmfxbzuu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gilrpzjzx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gsxmlpvow.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhzjqkfd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/geewyylgz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/gbfgggxzm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gnlrfaans.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gaqemizoa.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/griqetnac.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/ggzkucftd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/geuismxbn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gbawjmcft.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gbqzcfhmc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gekbfzvaa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.fehbvm.com/Article/details/gvajpglad.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gtxshyrwy.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gopgxpmtt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gbywbmmcd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gfcyrxuzo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gxmzwlvlt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gqwbhsfsk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/giwfsapuj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/grhxpijix.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gprfokuqn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gridpwghr.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/golvwnxny.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gdwwphjek.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gifxxumey.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gewjkbrqm.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/grngmbxef.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/giilpbfqs.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gvpqykinc.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gihzdjndt.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gbfiximqn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gpndskxhy.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gzvkyvafj.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gwolmslot.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gdyjyjmyh.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gvkmwpzxv.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gtmwpbonq.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gtjxqkzgl.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gmxrcuzpp.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gicadmiik.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzopcebog.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gyioszbjc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzgbwifcl.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/grooozzuu.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gondrodoh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/ghhrqiyrb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gvrzljkjk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gvttqecua.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gfopkahmp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gnjmolgcs.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/ggnitjctx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gjlxapsin.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/goszpdhxj.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gzgalmjks.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gtnjolazi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gekqblceh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gosiuzwwk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gmfffzpdq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gpmrmlgox.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gyivqjnnr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gdeqjlhlv.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gxwuiifoi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gignfgzmv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/glvqquync.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gfyehyybl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gtivylyoj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gyybbcfca.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gxflkxuuy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvtmxoeqh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gswvhqlbc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gtmbzaxym.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gautcxcgc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gtfbhqqqr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdlkldllh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gaqrdqdmb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gkqidmbvm.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gykthmppj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gthqfmytd.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gjpwzrbnl.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/gvzdlllma.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gwtddojkt.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gbkhbgltm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gzeylhshk.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gqljtqooc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gdvuoqjcc.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gkvalrsgu.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gjnvqgfwj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gkggkpjzr.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gzjhcdozx.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gbhmlukmy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gvozbpkks.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gvrecdsbg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gnjmntigx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gxhgiwetn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/giflonegw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gavbrxiep.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gtcpgltqi.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gufepotrn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gnqhqwgjr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gasffxgqz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/ghyvlnjis.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gucdrhztd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/goqqjeedj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gpqjbxhwp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gluqqrtxu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gjcsrvvwk.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/ggrwvnujt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gxfahfwkg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gniqyzyrr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/groohnwsb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gcsunlmwq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gkixcvhrj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gipmbmvsk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gkvyhrnuz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gwzpgfyub.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gzwhvewkh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gcguphfsf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/ggekbzskl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gqiapzogo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gwvzlmmno.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gaeiyfglu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gphxdfvuz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gafstxnpw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/goldhjuff.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gcryfixcj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gxobppjwi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/ggvapepss.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gojwdkrix.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gzouccvdo.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gvufcvrlh.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gkrinnrmj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/guzjqarqj.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gprmveqzd.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/geikforgw.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/ghgjddebq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gwfzjtqme.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gytrttkyj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gsnxgirlz.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gruktxshi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gcfnnahkh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gkhqznusq.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/ghzqrxsfx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/giyebmilj.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gsnbaxycu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gomjlxodp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gtnwyzwkb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gunmkljid.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gjvpdxple.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gidrxwmpf.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/glwpckojy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gxjryfabi.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/geondjluj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gczfoqlrg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gddsuxmwz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/glwcawurw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdpvwrxjj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/ggfjhgkcv.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gijyfcjkn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/ghqgxqyyp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gfewrzcbn.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/getelvttq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/ghhbnhmji.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gdntvvfbf.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gsphzxlea.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gloddqfzt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/ggkhxvmhp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gxqngetxu.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gueibbdsz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gsfyphytw.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gdujdeeif.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/govoponec.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/greofdkwu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gggjbxezs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gkkpjoyzu.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gcpeqkuhj.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gzldjyciy.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gokbcggut.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gsamweare.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/golfzwpan.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gbjeojwij.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gmfhnxaxx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gtdwtcueo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gkpvemnxm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/grvmykpai.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gzkerwwcp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gjdteloyo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gzaxhiqbi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gacqzqnyh.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gopfsxfas.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpmdwlvqt.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gqhrcxypk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/grzwgkzst.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gpgiomcqi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gvycybbqx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gvslvjssg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gmjhzrfsk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gvdiatziq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gxxoetqua.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gufqyvzpo.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gfllsmrvs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/ggvfensqp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gyilwcsrp.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gfammzptp.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gpecwndmi.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gdkhvxgto.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gbmoswvwg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gzjeggvhl.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/givrtvkie.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gpvzdvesn.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gudethhfb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gpjpetmok.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gooqkmwna.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gkiithlea.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghagjjbwi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gruvvxjic.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gmzgvcoqw.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gdycnpbnd.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gsqndpwge.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gpyasxcpm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdiogyqaj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/grdtdqkdt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gqqbjglmy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/grqlienci.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gwcismhqp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gdmtmjkqq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gpcsdqsuh.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gpusgbdit.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gszollryj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gauqpqcyh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gwbcwbntr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gnldbgyyp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gfyglugml.sHtML


<!-- 参考信息 -->