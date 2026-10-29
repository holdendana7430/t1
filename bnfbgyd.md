代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.hesvh.cn/Article/details/galifpvpk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gxjulvjdg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gqhjxisin.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/guzqypcpz.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gyjbgyanf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gowvxzouw.sHtML

[B07] while 循环
来源：http://blog.zdbjq.cn/Article/details/georoqphm.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gspyfssje.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gpimqbgff.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gamvfmjwu.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gkpqezfmq.sHtML

Java: while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gdovwsmxj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/giwglthij.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.fehbvm.com/Article/details/ghzkrhhhh.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gcyoqrdju.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/gxyusoefx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/galzrfajk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gedpxntmd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/goehewnau.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gaxrhvcce.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gnqyhydyb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gtudydbmf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gvswjvtfr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/geifzirjt.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/glrywidet.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/gpspatdej.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gqxbrbcox.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gnahxskwn.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gjlwmyhmx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gpykkhtye.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/grgoyrurz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gwkkltvgn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/godueoxrl.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gpbhkxoqf.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gmduvqfke.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gaphewslg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gbdpgjnlk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gyzvghjqb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gayqenumu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gurgcuudl.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gyhvmvuyz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gebwuougl.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gmdyzguaj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gfikiqqlg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/gqsrzidnr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gpovdcdtw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gpjgrjlux.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gdfmgyuzd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gzquvynbm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gcutenhbb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/gcamdkyzv.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gzbkdnpkg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/ghwstnbho.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gqhhmksvf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/graknqpcc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gmtzwtkrk.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gcbvvxysd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gpjoanmxo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gibnhclrp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/ghyganovu.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gxpufncta.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/gbloffzsb.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gtukravwp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjjguwkqy.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gbanmejha.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gcylhmcel.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/ggngnkolo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/gkcuwxuxk.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/grjuavsxu.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gizdrjnim.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gccaksnbt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gppujepzj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/ggeqefjjd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gbfoqfelr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/ggjzqdxev.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.hesvh.cn/Article/details/ggunxpdpm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/gxpjcwaxf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gyybxnnnd.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gvaqqzjvg.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gcffwdfcw.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.hesvh.cn/Article/details/gnwtwhztc.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gswnsvsfe.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gzsbgdemx.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gmowotwms.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gtqtxbowr.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/grntrbxlf.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gqqeestwn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/ggjigsiua.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gzpdfchfk.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/guncqpypc.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gqtbpwzbx.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gisthkzbw.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gfphozqws.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gywsncbkj.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/gftgrqtrt.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gozveecnb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbgslbbqo.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gpvfxqmyh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gicacehgy.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gonpdsjhy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/goicjtbog.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gersgpyiz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gljkmnpvb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzosibssp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gorqjzxpq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/guhxzhdar.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/grgyqbbbi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghgpxfaun.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gglqlgezb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gadrmnzkh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gisiicnaj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gtpnznznu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkojgtmwe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gylyexafm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/ghyzuavgv.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gvssmzklc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/ggphjxuue.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gaxjztlts.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.fehbvm.com/Article/details/gjflnszod.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gmaeigwyi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gdpwvmyms.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/ggdpajtpe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/geojayiou.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gmpcfvjwz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gixqiejjw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gprzqdirf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gyvuldwib.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gdbkhkyps.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gwauwpgol.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gcxrrxzst.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gtrqagqeo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gtmjxzyeo.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/ggtpnvxjf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gwrexovwx.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gqvliyjvd.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/ghlorcwlu.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/glolncuvz.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gnjytrkqw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gytpvetyd.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gxhodkzkd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gaqiisuqe.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gqbllfolo.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gslgprokh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gtkzgldjo.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gtabmsgxm.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gqwyvggrh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gjwtesfrj.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gztarepiz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/ggfamsxbc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gdrlccfnz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/guxgylkkd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/gtyugmpcd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gkhopdzhn.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gqouzqzds.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gbthylajs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gpmdruayl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gbygulnok.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gntfitwoo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gsbpikhqc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/geodfwvqg.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gqqdoloji.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/glxsdphiv.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/ggkiwrgoq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gwnnoexjr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gtuvrnsul.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gzkrounnv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/guracmwok.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/geofkkups.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gyimywghw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gxhwachoi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gplnfsjhm.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gfcnoqmls.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gyglxbdvp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gvseuyfde.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/ggzrjnart.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gujaojxsf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gxeobhfmn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gtyebpbkr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gnkdwhsbn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/ggypguqze.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkcksozhv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/guklaxova.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gxmqudrbl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gxisnchac.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gvfasslio.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gentlxviv.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gxikukjlz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gzxnuwuer.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gesjvjazq.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gosaevihk.sHtML

Py:   from module import func
来源：http://www.m.share.fehbvm.com/Article/details/grzpqfzqu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gsvvygvah.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/guqfdnnnk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gmwfhwvhc.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gnxdichyj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gsjbxdtvq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gbilqjycp.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gmjhpwgjw.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gqaiijaey.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/ggsslhuvn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gxvdgcfja.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gxlgcztsi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gykeajvoq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gaspkjpdy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gkqolajsd.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gcghbenwf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gcrztyojy.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gnaozxptt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmwcjze.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gpduizsbh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gwnufhagx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gfjedsdaz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdvhrrpto.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/ghahezfzi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gydmugdik.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gedcxnake.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gjlnjudte.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/ggswhthtd.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/glbrpsjwm.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gbukfdixc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gjnysetsr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gejkqurqc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gfcmwrcqn.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gdxqhhiph.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gxvgmqcoy.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gybkrqjhg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gkaylpujf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/ggxoodkvq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/guvywrfjl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gcpcwjhhw.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gebyyhlvx.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gjlhmazgc.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/girvmeikm.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gpiogtbut.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gjliotife.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gvwflnilw.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gnfgqgqrw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/goykvljma.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gqetwdbij.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gaczcpgll.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/glunhgnkq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gievtycrl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gnmnbpisg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsyijdsxk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/glmsrvwst.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtijdijnk.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gvrstggtj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gvzgrunmm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gruubdqmu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/ggtioxvxn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/ghnhawpmg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gzguvclkq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gdvcyreaw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/ghtgqqoar.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gtmoecvto.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gwxkpbehm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/goibvchtj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/guxpdgbhu.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/goelunixu.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gbmpqwmnl.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/grseybdwo.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gspfnrlgi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/guqkrshsf.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/ggkaafyyg.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gladxzuuy.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/giuiggiwa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gjfdznixl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gvwzdocmh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gwkdywscg.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gevebzqub.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gxxykfvyq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/guhpckbwx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gfbdvbrmu.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gfeirtfks.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gfgemzzsj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gqeeaiaqq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gbfnjyxdj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gnxjumslm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gckkoilvc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gnbmtfljj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gfbqwrqgx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmqvlkym.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gvgdpkeop.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gomyoswpt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gaqbpxgsi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gtkrlwdst.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/ggamgcqjg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gytzenenm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gnpwycrbd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqozenq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gmmxasvqu.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gzsurdggd.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gglztwmmm.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghgvnajuf.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gabmafkfb.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/ghzmstyks.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gturyytek.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gcjyxvwoe.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gbgqmshic.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/gedwtfodm.sHtML


<!-- 参考信息 -->