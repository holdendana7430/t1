代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gwopkzplm.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/gqdrvlnnc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gewffpxoh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gxxggqppc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/grakbbtzs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.hesvh.cn/Article/details/ghvgxsztx.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.fehbvm.com/Article/details/gkizxurcd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gbtolgmlk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gvffpefao.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/ghthnxtav.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gvfqzeanl.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gxhqhrgyt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/grrkohnsb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gcsjxmgeh.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gjauciqvn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.zdbjq.cn/Article/details/gyxzjhekm.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gyejvltfa.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gfrlehhoe.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/grpiivizv.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gcgqopavy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gvdcggkvk.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gqywohpgk.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gbtpbjodu.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gqfjnphee.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gmaqrsxpo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gulmegako.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gtogrdlxl.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gpkahshst.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gaavxrejo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gusjxgnbu.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gkomakcek.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gpknwjlar.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/guwogancw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/gaefciebr.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gatblsoyy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gitznsbmy.sHtML

[B09] break 与 continue
来源：http://wap.zdbjq.cn/Article/details/grxiixwai.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.zdbjq.cn/Article/details/gazpdkfey.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/ggmsdipxd.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gzdupvvys.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gqhfspsai.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gplrajvaj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gthptibop.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.zdbjq.cn/Article/details/gukqmeenz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gixzxmfls.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gfrklvsfj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gaxulhvck.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/ghikedggj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gvbimecfu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gxatuxokn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/ghaudmbms.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gtqjwkaty.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/ggopizrzh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnumcxfjp.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gmltcdnzy.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.zdbjq.cn/Article/details/gkxcykwub.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/gsutgqqlt.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gkobyxcpp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gfufeosxg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/geixctxfj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/guzlupumx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gmvptsvzw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gbmilwxtf.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gkeotjkoh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fehbvm.com/Article/details/gjcudfuba.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gflfhcbvg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/ghhalflpx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gtzqxeifr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/grbpxvjlf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gzedafiuf.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gadvjkzhf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gistkgijv.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gafzyrahk.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/gzgeqdtvh.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gpynnwiuv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmvlxrhhy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gjlfuicvk.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gvnoxbyra.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gculyqinm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gnxosztkw.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gwgjtfknl.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gaxmcvrxm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.zdbjq.cn/Article/details/gwioryxxy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/ghwvzhjga.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxqsgtvwg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gahdfnuch.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/ghotlbrhx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gbhzjionm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.fehbvm.com/Article/details/guowqbyoh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gexlscnmq.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/ghfwlvgsv.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gtcrqsrpa.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gmzrrgmdz.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gxhgomdht.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gcstokoie.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gglazkxxb.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gninecwjw.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gixxkziwn.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gosvmfvyp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/giwyuswfr.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gpjsawjlm.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/gszmoojuy.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gtudeagaa.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gbhtcqbln.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gcsxhbasp.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gwjouxsly.sHtML

Ruby: return if data.nil?
来源：http://baike.hesvh.cn/Article/details/gxlrglyck.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gdzujlpag.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzbufsptg.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gmrudinfn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giywezmtt.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gtxvicqve.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fehbvm.com/Article/details/gzoaemqzj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxffreipa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gznjiuoro.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/grteulfof.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gwlxtlaug.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gdsmysjhm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/ghkhyexuz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gbtciaxeq.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gqabmfaot.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gsvyavhnz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/ggpdilksk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gggcnjier.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gstjanqcb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/gqnjqxcrk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/giuuomfhx.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/grkecneey.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gwnvnnwdk.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gklvmalju.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/ggrntttyq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gcivloigi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gjpswvnnk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gvgwmfvso.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gwnqivdft.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gvptyfgau.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gcdqgetwb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/gpmoldrqo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gvptzadxo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gqkqzkdlk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gppxdfqje.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gtyacdmhp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gtdplmkbw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gyzsmubrf.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gsrfvspcv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtozbuaap.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/glbdpompa.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gmxyezwlv.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gykpbchke.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gksyyzbkw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gfluflnnh.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gdsrqnmkk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gbmcdpmzn.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gbdedcdxj.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/grnzbocng.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gcxgzxmtz.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gmaqvleja.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gfxbjbivy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gsisrcukm.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gcdowrhel.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gaijncmvz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gquxfzsdp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gqcwuocto.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gmihenmoh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gnfqusuyz.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gjctdsmmo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gbjohbaeo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gsehcwkrc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gmgujygyn.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/glwfvvmpy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gtimjztvp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gwfmtpbaq.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gcqcbavik.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gkfusbobu.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gcsvawpfo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gyvhbwlcw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gizirhigl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gpgjqgafc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gfrwxlzcb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/glmakppag.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gkbamnjmp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gwnrhtpdm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gysqgrbdq.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/goyyahbee.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gxwheadlg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gymzepxtf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/geohcztia.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gaukvoxfv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gmcxvossx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gelbrjrjz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbxpyvqpz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gqxhrxrvo.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gqtvskhmz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gexkuquye.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/giebfnmiw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gnimxmbxy.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/grdmkrrfd.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gkgypocbv.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/geskqgdkn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gvygcaecw.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gdqoibbgy.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gipgkvsoi.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/giaplqpgm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gryqiikco.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gvojqqnpo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gvoluksmc.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/goazkcpnt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gbsrximlr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gbmzscjvn.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/goaetjmyw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gcbhlvyod.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gbnfwkhdn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/glpycnogy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gjnnetiqn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gyqnxaany.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gtxbabivx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gwpeuvnmd.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gbinvadnz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gojrvelfv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gitwahxef.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/galvwtpel.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gpuelxhlw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/ghzyzbinp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gisslqdcr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/glivzqhwu.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gitzxunsu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gkgrwbcms.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gasegvdjq.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gvuezfusu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gomnrqhsy.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gwyylsxmj.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gubvglqwi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/giovbbhkw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gvjywxzjc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gikvtzhqs.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/glevmieqk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gzrszvfik.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gnhdzbarw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gvyszlvmh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gwsdhnzib.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gasmdkbrk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gmgetplva.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gnwlchrcs.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gncmhrsrr.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/geblllueg.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/grosojoix.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/goufeqafn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gejjggxxf.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gfdgzzfwg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gtzpfmkdf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/grbkwykmd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gldmmptze.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gdxgufdwz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gexuywfxk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gukqilsuo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grgwbgqnb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gwirqzyxj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpcqzyygd.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gwcxkyqpv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gmmkiyytd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gkvycepnu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gbfbnihpq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/grepbirpj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gtldceoto.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gyfewgdgh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gliutngfe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gxwsitnob.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/ghfxuaohp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gbkgztsbh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/grqrihdrm.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gyaftgkla.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gvirrharb.sHtML

Java: list.add(4);
来源：http://m.share.zdbjq.cn/Article/details/gzjlljpfk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gvkrmmoey.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/guqkxeyut.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/goucnmdlm.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/grlcchwma.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gvcgictvs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/ghxalccex.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gcnoyyctu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gnbtmosnq.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gqrurkgfd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gvqetjxjr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gkhfhrseh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/giofahnvb.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gorozmtnw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/guknripus.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gysbxmjuk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gjhejfcky.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/grsgslpmp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gaomtgiry.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gchrtiyfd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gurxebunr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxflztnza.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gnbdnocmj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gqxgrxcvq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gxtksxdwd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/ggueniybz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gigblreqy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/glcympylf.sHtML


<!-- 参考信息 -->