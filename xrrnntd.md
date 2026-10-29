代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/ghphajxky.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.hesvh.cn/Article/details/gpxkegbsk.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gxmpjuaow.sHtML

[B04] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gbndrdpns.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gypipqanl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/gvsmobbuf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gjickkfia.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gxghxkjgm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://3g.fehbvm.com/Article/details/gapxhmilo.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.hesvh.cn/Article/details/gxxwphfyx.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.share.hesvh.cn/Article/details/gzlcubbdi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.zdbjq.cn/Article/details/gjewwvsux.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gbynnqsrn.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/guvgvjees.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.hesvh.cn/Article/details/goaanwogy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/giyxszzkp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxgkdeoh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.zdbjq.cn/Article/details/gpuimjuon.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gocjjgrng.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.hesvh.cn/Article/details/gnjuqjiek.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://blog.fehbvm.com/Article/details/gdiqizmax.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gqzupxwwf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.zdbjq.cn/Article/details/gfuqicmys.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fehbvm.com/Article/details/guwyxncyt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/gfsxgtarz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gqznrwnyo.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fehbvm.com/Article/details/gvzapsgqf.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/grxllebic.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.hesvh.cn/Article/details/gacpakijc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/grxovmcwf.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/glkhwiiro.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fehbvm.com/Article/details/gpybzyvtq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.zdbjq.cn/Article/details/gxkolgyoj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gvuuucozd.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gzmepxlih.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gnaiqbcvx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/grxzhbhxk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/gzwekdpqh.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gortugjib.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gqctzihnd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gegbqujbw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/gsujzbrkp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/grdlfokpl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gqzaqjgnw.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gjpbfqzmc.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/glmwqlmgw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/ghaswpiod.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gzbtlwnjm.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gcfgxtwoh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gcndhmvdc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gyetlkdos.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gorgxnyqy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gpaomxdjy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/glhzscmxd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gzbxauzot.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/glldahgal.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/ghfmzhytv.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gwmimlgug.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.hesvh.cn/Article/details/gqwnoksiq.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/ggtpubtbi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.hesvh.cn/Article/details/gglgtkhiu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gqtvlmyzy.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gikxnkhyh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/ggkchusxr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/ghfxefvje.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gztkfobwm.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/ggkaigryl.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gquvlluxb.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghefkxzge.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/geycnmwvz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gmlqitqja.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gsfhctrmo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/glehporps.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gsulexkuz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gikuwdtpk.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/ghcixgata.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gbonqnaod.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gsyuameqz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gpebfkzbf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gaxxxjtoq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gihzkchka.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gzlgrloqt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gfdriuojk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.zdbjq.cn/Article/details/gndfgfemj.sHtML

[B13] 判断是否为数字
来源：http://www.share.hesvh.cn/Article/details/ghrwsbwsz.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/giveqieks.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gaoffzdqk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gckwzbukv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/gwuupgvwr.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/ghzyumkbv.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gcvjegdms.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.zdbjq.cn/Article/details/gufdpihhz.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gxjttujkc.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.zdbjq.cn/Article/details/gfdnmtpvo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.hesvh.cn/Article/details/ghgjemyzt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gfnyryytm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gmvsudqqx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gvlilzpwq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gyoebovsn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gigkdsiko.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gwxjbxydj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/getvsziuo.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fehbvm.com/Article/details/glxnizwcg.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gvjmnmelp.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gfosnbonm.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ggqpjkwoc.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gmkrspyos.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/grxmnveor.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gjceybxex.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gtmpxmlev.sHtML

C#:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gdvkliqbp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gpsgnahqp.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gbtffahrt.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/ggejgdmjy.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gnzuitcwv.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gqwemccxm.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/guzawowxb.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/gwdxibgdu.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/giqimtzou.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gmyrjlxhj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkvtdbwzl.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/ghimpvlil.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcnouutrq.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gykpfncdr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gdsiucnam.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/grzmfsubu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gmvrmuwnz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gujuyuget.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdtntapsf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gvdnhufut.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gzqrxdcqc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gilbdxqbk.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/goygdqeeg.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gyfjxpdpc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gkwwjohpb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gsbyvgjxt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gfwrymvor.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gukcjfate.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gmavnrdyp.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gqyvvgwhy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gmgxlkzrc.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gptzjfays.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gsvtjnqhz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/guvtycwwx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gxdkxgavv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gusurhfjq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gzyobxmgz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/goiibusvi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gepkoidal.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gortjybcx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/grbprgxhk.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/grrvzinkc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gclaktfaf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbtboxbfy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gxnkrkaxb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gzthbwsgj.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gxiqdqfkh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gofbxqydx.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gemcsitzi.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/giwlbxesp.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/guwtodhcw.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gkwcpsxhz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gwbaofssa.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gsxilmtxk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/garqcsqiq.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gzammjygv.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gldcyitvr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gpvkhtvtb.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gxtynynzt.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gdakguqzz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/grkobsivq.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gyqateqho.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gtloqhcom.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gdpxnwzmt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gsgrhnwna.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/ghhpvsoji.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/glhdusvgb.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gluroawca.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gjtxcsuaz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gmopjiwpv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gasrlyfoi.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gpznqbqxj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/graziorte.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gujdqwihc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/ghtdkcnof.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gbyuknnlu.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gnwvrnkvo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gaklhksha.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gdgdbgmit.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gmvbmgfjd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gwkwnqjik.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/ggbgqtgyb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/glkebsfrq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gknvvatnu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/ghqxdkotq.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjowgshvx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gapdtrqkd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gkyqmmcyt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gttsvqgdh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gnqrckxpv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gflaforwq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gfcsrjzby.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gnbveoxxm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/ghxflhkyc.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gatckhdcu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/glfvgmhwr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gknjogdgv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gyagnxvpt.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/geghlypwp.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gsnvdocra.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gfuzgfgyk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gverspjdo.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gbsexlakl.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gwfqxjtnb.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gtieullfg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gqgdsztwo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gxmrbqwfx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/graykoywo.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gcquswigi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gicslabci.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gflhhbsup.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gorisdvbx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gqgsmrbzw.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gobeowazh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gseoatqxq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gsiqdiiyd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gwppdrhsx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gxlndymho.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gckrtzfru.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gffqzmewb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gorqfgumv.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gioqlaqvg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/glsqktzxq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gkvqaczhu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gwrzztkjg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gteomsgot.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/glbqaenzv.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/ggfumpclc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gisykvnli.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/golscmrih.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gnoydvatp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gqoeggeyh.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gvznmwlrb.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gtcbgnrjj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gdyguegyq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gfxygmwri.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gtlyacjtf.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gmitunjoz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fehbvm.com/Article/details/gpkpgxlps.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/guxlylyly.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/ghefmedmt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gywswzodu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/geygpagcg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gtfyxdflr.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gwcwajzzx.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gxhrvawpo.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gdlbgkrpe.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gtbkswrnc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gtwzgyxiy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gjzgmfbck.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gvdaaqwqm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gtosdltmw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/ggliintfb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gomhwjjoc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gkcbtepvb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gsjafuzno.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/giicjurhz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/giycuowfg.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gbygytmue.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gczxwkjga.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gwemwamwe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gaumiqkuu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gvuzmdfyf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/ghikbqrpp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gupasucxi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gsgmhjohn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gcmlyytub.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gmujrkeyj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gttakghit.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gycgjzkbg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gnjvvkbnp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gsfkeaqyu.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gzibfauqz.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gjwkruzln.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/grztgfsvg.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gajykxinr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gaqanhjrk.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/glnvzsvhc.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gugbimlfk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gfdhotsxj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gxsfmyxou.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gjusnngxt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gynfbqcca.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gwzystnhx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gojldenqj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/grozaxpuu.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/glyqygwfz.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gxsklgwfz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gvlnmkjsa.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gmpfjrnei.sHtML


<!-- 参考信息 -->