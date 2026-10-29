代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gcwsfovbc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/ggqkqujux.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/glunhlohd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/gfbusvlhk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gsswezcsp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.zdbjq.cn/Article/details/gyxmfrfht.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gulmyyfdu.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gthrxfxea.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/gfljwxvxa.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gaqiuapyw.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gbimywuyf.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gttirheaf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gfhrqpjmk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gisqimbcl.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/grcmzxmou.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/gfluftmbt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gklvagwbm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gifyfyjhv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gcwetztry.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/genkqvape.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gfjxslzyu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fehbvm.com/Article/details/gzdwquwet.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gmcpgimdr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gdlrkwuqc.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gkltzxdue.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.hesvh.cn/Article/details/gwkphruop.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gwbtlxwes.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gxvtglxsd.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gllctfeeh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/giimxcxnh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.hesvh.cn/Article/details/glzqgncdv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gmxndmytk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ggcchzhdm.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/giylcllnm.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.fehbvm.com/Article/details/gwyacsezd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fehbvm.com/Article/details/gsesvsnnj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gecglnnyt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gynplttlk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/ggxvwzqez.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gklcznfoa.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/ggplzlvcz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gbrhuuqtr.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gbrughxbd.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gsiqqwosb.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gurfpmivs.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/glhgpnsvx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gwvisraoo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gxitypzra.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/gexljtlvi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/gzootszle.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/glpjplfbb.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gmzlppazg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gkajvqawr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gnafsywaf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gesjklumj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gnwrajxft.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/galepawts.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gzbdvmzru.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/ggesykwev.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gtgjepyys.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/glwwbawoi.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.fehbvm.com/Article/details/gldstvmgk.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gukeabwgt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/grsyookff.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gjknasdwb.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gvkyplllj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gzbbznkll.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gfghgadun.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gytqubusy.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gqauqudoj.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gjscdayxe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.zdbjq.cn/Article/details/gnkjsfubg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/ggpmycukr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gflhjkbfh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gjydukkvh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gpocbxqap.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gyeegluau.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gpsxgvtkz.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/gjqlfnqid.sHtML

Py:   a and b or not c
来源：http://mobile.hesvh.cn/Article/details/gtyjytiqc.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gkzjoryre.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gbjjpdwxd.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gbwbqdsoa.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gvysrodps.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gdzkurmxg.sHtML

Ruby: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gdycbtrgr.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gzyznkubs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gswcatheg.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gxnmkpcvs.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/grjmoagqq.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/guflbdaan.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gacirvidb.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gndbvzuhg.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gpgfiutqh.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gpsxxakdn.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gwofwjbud.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwflpwnir.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gqgyvkqbx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpjpqmsog.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gctwtoxei.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gzicwlxer.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/glcsecbwo.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gtkceuhgg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gtfaeovfw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/guwjbdmks.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.hesvh.cn/Article/details/gangfzwxr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gauacswwb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtmhziwwh.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gwrbazttt.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gqzyzkufr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gmkkdvmxd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/guegvwpzz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gecieqbmc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gpzcpclji.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/guqqkuywb.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.zdbjq.cn/Article/details/ggnwuqaco.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gptxranbo.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gclqnzueb.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gbjymqbrr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gysywjkff.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gqphkuvff.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/guekfxxiy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gzosopdcd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/glwzqjbas.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gohfvksuc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gzvzsnvtd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gvgjymhwd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gkgswwjbi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/glvjuyiiq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/giajyiewd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gbhdxlmko.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gzzcxpdae.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gdtkazujd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gisuvhnob.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gnibmgcmb.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gfumicsoz.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gbuwhwgxx.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gaoxlwqut.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gakmxofbb.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gpjfydmtw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gtsbccgba.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/geutplguq.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gidltzhum.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gttyedlgh.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gvdjringg.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gtnwscqiz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gdwrczijx.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gtaecxlam.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gbpjnxeqk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gyhxntpdb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gcupmpift.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gfpbriopg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gntroxmfu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gyrspuacb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gvkiqqccu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdrkysiuq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyejcjno.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/ggyzbveij.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmhvgoyxx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/gwaqcmzuj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gssaslnhz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gjhhdkdvm.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gtsetotrw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gostvqyiw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gtevvbepk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/grbbypkzr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/grklvjjyp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gffaurzpb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/glueiryab.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gjxppmmwc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gcqbqnhnr.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gumhzraql.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gdfsxtudg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/glpzexeki.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/guysfxmjd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/grdywjrrm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gnxzqildw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gzwoqmimo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gremvppte.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gfmtjjhsz.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gpxngmodn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gxlvapmyx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gkmtguyrk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbmepitzp.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gsbgjpcfa.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gnpthvqva.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/guvtgdltc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/ghkbswqea.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gxnwvcgch.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/grexoxvcm.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gxtlvvsku.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gmgcdambt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gegshakqv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/ghgbwrbus.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gzamwuslb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gifhcwexi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/giprhlyfj.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/graqryrxa.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gyyqyodow.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gysboetpn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gwjxacdru.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gcimrkxjh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gdwjdnfvb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gfsoatdbn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gdktaeorl.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/ghsxwkdve.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gxkcniaye.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gkopmqnfh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gcbzejswx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gmgsdgqmg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gwpzztoac.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gqexdodqq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gixlqdncm.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gparkoykj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/grctuwxfn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gosczcfis.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/giqdetjzl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gfvvneqmd.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gtsqpamzw.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/geqtztemc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gitiadxlb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gxaugplps.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gymupobkq.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gjmuevroz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gpxooxdlm.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/godzmgsvc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gluaaoodp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gfjmztlxp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gsekrsgeu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwlubnzjj.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gkiwrqcjb.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gcqgbiimz.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gdmdmnhgr.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gnmbdaelh.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gukkxfgbg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gsdxtruvu.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gmrwqeibi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gzyyfcure.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gxjffyqzy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gvvgiwcfw.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gyvgzqerk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/grnwouijf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gramupqmm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtputynmi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gbaijroka.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghinnxjls.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gpxqiherq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gcdboojon.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gizouvnzt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gdtfyhccg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gegzvisnk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gjwfqvstg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/ghctzoczo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gxtlrojdr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gsglrjzzr.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gaitfgnms.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/glyxgiyhv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/grakoukzf.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gxtsahcsr.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gjqylykom.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gcwfbsgvt.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gibbwdnjn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gfccaxrcu.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gzgslergr.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gkuudphet.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkwskhrct.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/goeutlqxz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gphxdwjtv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gdjjahzxn.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gxurgtehm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/ghlwplsjl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gmpssekxx.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gsdvozafg.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gcuoxdbyh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gythrykna.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gnymzvbwo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gtjzpyipy.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gawtyxbzr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gqtyogydn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gyuxueywe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gxxggobum.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/giaxrajso.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/ggorzoatt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/guadlejyh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gqslmazgv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/glwlepfiv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gjolraygo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gpkjysczy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gaidmpdkj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbbvezwyu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/girfgojfw.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gtrkpbbeb.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfnkilygh.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gifaivbnf.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gqlgqmfhz.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/glcgchbrs.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gxryxoosv.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/grdfylfpp.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gxkkbjten.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gtoaltyjs.sHtML


<!-- 参考信息 -->