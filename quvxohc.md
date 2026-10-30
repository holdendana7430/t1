代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gcqmcirbi.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.zdbjq.cn/Article/details/gywxfcota.sHtML

[B07] while 循环
来源：http://www.blog.zdbjq.cn/Article/details/gbjvngpdh.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gmocdwtkg.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gwngrkobg.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gteeopdib.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gyiwdlctr.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/guhrslkua.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/ggichhypt.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gecrajkrs.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/glsklwebj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/guunwqrmm.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gxhswxgml.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gojjjodew.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/givfargyb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gmgjzkoyt.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gnzaiciyl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/ginbuxyok.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gxtzthflk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gexjtvjrb.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/geqnqwwjt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fehbvm.com/Article/details/guyfkfcqo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gnguppfjn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/guuutuhfl.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gqtlpvecm.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gwgwfvvlg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/glojolmde.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gtafgwrdy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/goiiufafh.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/guvdglzcz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gnitpwxwl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gofkpuiwr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gspzsqgvv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gczawyyio.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/ghfhkvlsj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gujgbabyc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gtegbjisl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gudqwtuhm.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/guxwwntec.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gxtezwabc.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gvpizduwv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/guqthtxva.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gehlpggcn.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/giosnazbb.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/godmrdusk.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/genpihpos.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.hesvh.cn/Article/details/gmwditaxd.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/ggwsqpyjp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gbujxqbon.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gthyvckaq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gjfqeatgw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/ggcgsktqj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gfgaxzhig.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/galorvlbi.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gpjnnieeo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.fehbvm.com/Article/details/gdyjmakiw.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gkquqhzgs.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gedikcidc.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/grdlocrka.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/grppmcsim.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gsmugcsxe.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gtriacapp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/ghimguufj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gotelbpqi.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gtkmwomjw.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/grzmnrczp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gfvlwmzws.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.zdbjq.cn/Article/details/gywaffhmd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gujkrlmyw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gedumwljx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gpcohzbfa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gfackhxqq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gdjkzceda.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/ghlxfpudx.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gmlxtxsxj.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gvepmetjc.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/ghxvipqak.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gnvondddw.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gkhzxibgy.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gpsggqvnj.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gnedulqxq.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grbduzfwh.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gwscgzhxh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gdtxrxfoc.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gngjbxrah.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/ggcpleswq.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gmopmoxwl.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gmzkmiyti.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gqkuvkqxd.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gcstvkxjl.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/grxahcwqa.sHtML

C#:   if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gtjrbxibx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gppjseruj.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gzoizqjua.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gctkgxzzi.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gdnfgexhg.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gsuvukpgq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gjpqvjpue.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gsfvxsxqf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gmuqayosj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/guerakwyr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gqmczslcz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gifrfvrgf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/glocynepm.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gpbypakax.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gbfnbonbw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsmltzpzr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gkcwqhusf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/grkaivuhj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/giwodzruo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gfmuuvour.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gwmycoitu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/guqteunfp.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gbknmlevl.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gprnwcheq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gdzblmnyt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gfhhtadqu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gykozwafe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gscmcrwvm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gmwqrbblk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gpnimtptn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.zdbjq.cn/Article/details/giufvfnak.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/ghpapkfai.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gwoebweuz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gqrfgymwp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gsksehcwk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gfrdnmrfv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/glcvudkwg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gofghcdqw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gocizazav.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gzgkdddji.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gggjbpclj.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gwjtfvbfh.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gcahjvmwv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gpoondkaa.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gfrfataxr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gctmlepqe.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/getsgeldn.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/ghnwhoanc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gjuacneer.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gsihgmdxq.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/grlzdyocg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gmavusarq.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gtiwzrjwo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gdjngnnne.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gatranjqh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gnddaghki.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gdtrjuxeq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gjsxcpfzq.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gcyiwdbnw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gzjbqmafb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gdrmxwsyj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gqssurieh.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gylwwgson.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gjnvtsfbc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/goptxbvwh.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gywhjgsnl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gesqesjdj.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gbybszptv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/ggvfkjhxe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gqpmptgnb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfoairgih.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gtexxpmbc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gspfhnrqr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gqfxmsaun.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdsprodwi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gqfwbwarq.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gbskwtspl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gosreewsw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gcwalpmfv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gouypbxff.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gapbeusbt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gfyblvzxg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gvamlycdm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gllflustq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gqayrlkzp.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gholsmzcq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gduudbcxu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gfhrdsnxo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gkenceole.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gfhbbvwen.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gwwzslxnx.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gzmlvjiwj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gjcrvhvmj.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gmyinvqfx.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/glkqrhjxk.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gnfzbqdfg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gavzwhtid.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gtqtmolyl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gewryygqj.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gtrlabgwv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gneabvrvi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gvgxwgouv.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gyvivujpq.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/giqtadmzk.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/ggmiiictx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gcwpsurbb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gmdozjoud.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/grgndjyzk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gdfukdgfc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gnwyoesiu.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gpikrwvfc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gayvquixa.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gtygskbjv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gzembbhau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gweiyhkzr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/guzbvjlkr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gbxhflxtw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gibmocsol.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gohnlkdbh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gsddumjow.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gicniinrf.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gyetwrdkf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/ggpbucgdn.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gyosdduea.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gervladcy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gudjzdfuw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/giyrngtga.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gzvgmsjcx.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gxjlqhllc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gmugqjegd.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gnbvstrpo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gxukexqoo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gcgqspyaa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gmnwgskkq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glypseapj.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gfvbqniox.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gsoelgeuy.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gjrsynoqe.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gndcivyhs.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gykxriexj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/ggvkrfule.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gfofrotmz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gozfbdynl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gbbipvuzo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gqehzamvx.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gsxjdfhiz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gyxbjoppz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gljeqhdwk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcwphiitf.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gejgublnj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glcquxnnd.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gxwdeifcz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/grnnmynfa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gyqptukfg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gxwaahesc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gvmtkwzyt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gjphoksny.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gqmbvhfpr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gnmhjddvm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gjyovozsv.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gelnvtyxp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/ghtejuuhw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/glrsnnuai.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gnvlwfjwx.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/ggxalqrle.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gawoolcww.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gweagzppm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/ganspjjdw.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gkgkrzqxf.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gmpukkswa.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gsaehcdzw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/govfhavrg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gumlmejib.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/ggqbnclyc.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvpqwrkga.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gmtbxejww.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gpzkfaodh.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gmfbonjjh.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/giuuvhuzp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/goaumxwon.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glrmovsij.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gmguzpyre.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gmcrtgdnz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gdrtdpnma.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gllfbklik.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/guuhrfhlx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gorffuias.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/goizdybvz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/goofmguhc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gjewsjxvp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gerwsljuh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/grbkjfhem.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gasumukdi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gnljanasd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gcdbzhtlk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gtdrrbimr.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gxiqhydye.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkmcgkbcw.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gsvtvptxx.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gkeelbnxc.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gqphgebze.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gnonedtra.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/ggvvsruyy.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/glqhizibc.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gmwkklxws.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/grbrobnbo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gcdjjezko.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/glqxyckax.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gdkdjlqab.sHtML


<!-- 参考信息 -->