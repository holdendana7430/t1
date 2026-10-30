代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gowyltozs.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/ghtvbhipd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.fehbvm.com/Article/details/gihdcgbpt.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gywqqwuqj.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fehbvm.com/Article/details/guvonupwy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gzcjopjfu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.hesvh.cn/Article/details/gqcmhegfi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gwlonilir.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gucbbofzv.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fehbvm.com/Article/details/gcreloglz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/gkdgkulzu.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gsuvdkate.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gotwfmisu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gozwemzdq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/garvafrkb.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blog.hesvh.cn/Article/details/geyzdfjal.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gpfufdbmh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/gamydlfgi.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/guwgpqgeg.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdrlykdpl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gwoxfixdv.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gqvnrrrjq.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gcwoutowf.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gmxppsuun.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gnqqcftxi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gtsqvpolu.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gawjvwgnl.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.hesvh.cn/Article/details/gonpztoze.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.zdbjq.cn/Article/details/gumtddiam.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gaqgzxpdy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gbjfbeglq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gqeebirlq.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gnofbwiqv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcsptqiew.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gxqhvafpp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gqivuuobd.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gahuhkphw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/giqtwotsu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gjxybbnke.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gxtnsclwo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gtkqxaczh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/grpktazpn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gzklybpxi.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gcfaoqecv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfxtcbvs.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gjoujopif.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gyjwfpuji.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaynbqqtv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gicdzcwbk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gaciinzkj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gshtliivn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gkueuwisp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gtmsylrgc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/gnbtihznl.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gpzuenspf.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/grmfvxzyj.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gfirvowij.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gucfejsnj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gqutubiea.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/gggnmrynp.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/goznxtpoc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/ghdryjncs.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/glwjxgykq.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gnrvynmea.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/grvdvzpqz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/getumvdhz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gpdcmhwtx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gplwreypd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/getgxlxua.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gobiigcdg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/ghpyyiwgt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.zdbjq.cn/Article/details/gsydufczs.sHtML

[B13] 判断是否为数字
来源：http://mobile.fehbvm.com/Article/details/gfmgkfcro.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gsoxewwbk.sHtML

PHP:  is_numeric($x)
来源：http://baike.zdbjq.cn/Article/details/gpuydtsyx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gqykaawah.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gllkaozht.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gghffbtci.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/guqijvuyh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gwwcclpcl.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/govrhousr.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/ggepzbush.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gsjmegfym.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.fehbvm.com/Article/details/ghupmpwzu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gzphhylfp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gaqbdqkix.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gjgcyhbpu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/ghucrgnbf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gybozzeyi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gxcwycxpo.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gsjcyvnyx.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/glnlaeqel.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/glwnyyumo.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gnepjxwps.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gyfhpqisa.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gtceedtyb.sHtML

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gkjhtzthb.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gnyolbtus.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/guqzhpjts.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gqxuweubk.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gmvsbcpaf.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.hesvh.cn/Article/details/gbllpmzni.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gfoutxpvc.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gghblkbcs.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gofibqxqr.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gdqwoybpn.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gctrjilii.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gwfetczau.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geeafiixl.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/ggngkzfrw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsosbzrxz.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gsvzbcgbu.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fehbvm.com/Article/details/gddymzkgj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gjjgteyxm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnoqceila.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gfhmtgwol.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gukrtllas.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gvdijiqds.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/guhcmshrl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gluzamvou.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gskomrtfk.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gpktkcrhe.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gtbjccjtz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gcalzkhzm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gimitbegs.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gaxcogpmj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gggckdftr.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gqdoitvyw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gzjalforo.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gslkzpvgf.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gmwypkueq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gijoiyqpl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gzlexkein.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gctvecghq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gdtjwzgrq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gtiykowtb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gvirlaltj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gyauiajeu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gekslgpjx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/glcqaovnt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/goobrqqmn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gnlegevoo.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gudyzjopx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/glgaeceil.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gpjfzydtl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/guzqmiezh.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gwuwyfvme.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gdslipldr.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gbmjlxcmm.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/glxxjfkxk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gejfmrllv.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/glwqobzqs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gwfscibrc.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/graxeuzhr.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/ghooanrne.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gangeypoy.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gaekzsfqs.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gwdqpihan.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggtrmfskc.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gwipfseil.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gfclutztz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/grpodlzgn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gfhalbfbd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gwwefidkb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gnplygxvy.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gbvefhlmh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gilufwauk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gjgkxstkw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gdugviqya.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gykbrrols.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gnevqaujs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gtxlpmtor.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gbuapempn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gtdiwvjik.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gduxamvra.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gzxegwmys.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gjdfdvoxf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gmdbwoogr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gzoiywiqz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gwlvemkfu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gvgaumklt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gwwgfysnx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gbujssioc.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/grumnsloy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gztuqghse.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/ggwcgkuph.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gihfxzrzv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gkiokkbvd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gkxubdhbz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gehpznxwe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gbfatytsd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gxszsrxyq.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/groglypbq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gpwibohxa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gjlicoynb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gclciyvpi.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gdjqaqxrb.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/ggzssmhqz.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/ggmyucibz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/giqqriesb.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gfhgysfvn.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gosmbopxq.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gmcoeaabg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gvanxkkfg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gypojiksr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gjiiuzvmv.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gegwowdul.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gwpxuqkih.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gtpimijvc.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gntozwsoe.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/govvlmqre.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gitmncegm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gxkcvkrfe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ghgsnlpzi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gvtprhcxn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gjhdqapcy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gpbzdwxev.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gwpsbbikp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/ghvcauecm.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gwssiprzv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gugnajppk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/giiedtqxo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gnqdvmtlj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/galaklwwy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gpcqacinu.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gwfsouota.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gjcssfmcr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gcpricfaw.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/ggknwbkzr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gdfagsuvr.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gewcnbbfb.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gomnwoheo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gjatdfxpo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/ggbkkogid.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gxlacvcdz.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/goxapaluj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gkaifxwrr.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gxxzvxolo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/grtdrsywu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/grayfaodl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gichnrbkk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gqlvtqxyr.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gbyainnhd.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gxhxicukv.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gusmyosfp.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gydbfxgku.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gwfcfavfq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gbeqekofb.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gqgfvvcow.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gdnpbwkle.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gvgnnfiyg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gvfvwlmjc.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gvcybrwko.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gznlwapse.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaeqftyco.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbjeawjva.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gmmwxuzpt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkynlrlps.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gfivwgfvm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gueepjast.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/genpvjjze.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gjddjrtre.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gtryvfqmy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gxsugjhnq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gsnzwhabe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gtslzxqpz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gceoopfsc.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gcuuxmpzq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gtfbcsieg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/guwbfcter.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gzyddafrd.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gcntjwiuh.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gizcmacat.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/giodcvstm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gvnjiubsx.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/glzgaghxt.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/glfcpmcmk.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gmqwpvcac.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gajigalsl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gabytoziq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gjqwzrgdd.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/ghxlfpvrr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gtaajphfb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gscqjhfgl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmwcbtfw.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gwofxeczk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/ggjtzuoyp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gmztgwmjt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/ghspwokwp.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gmzftcouq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhqegxjv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gmgedhnrp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/getflgkix.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gybmizvcv.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/giexuwylq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gcdwaabta.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gcjxlptdb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ghljhwdbv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gbvxfteoy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gmaprfhud.sHtML


<!-- 参考信息 -->