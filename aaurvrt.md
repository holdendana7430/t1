代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/ganlarpby.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gmemnjttf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.zdbjq.cn/Article/details/gmldnqzyi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/goblcqets.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/ggbswpjcc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.fehbvm.com/Article/details/gdqcbjjbm.sHtML

[B07] while 循环
来源：http://blog.hesvh.cn/Article/details/gmmvgoocu.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.zdbjq.cn/Article/details/gotnecouc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gyeqlhmoe.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjixckwze.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/goawfktio.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gtwptwacl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gyywyqpfg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/gwyjrrwld.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gutrnomme.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gwhaonwbt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gyalnzike.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gzkffhynp.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gigtzxunt.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/ggimjggoe.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gxqbafnau.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gahzsfpix.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gilkzgmzd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gmpsyqjbt.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gvtpnwoul.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/ghahnxxlj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gagnvmlgj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gquzohbpq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gighliijh.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/ggzhutsbd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/grnwygdzy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gmmgymmhr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gatqcqjhg.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gphjcmuyx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gxxorcsuu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/ghifovomk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/goxhkuhnz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gcgynzrbl.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/guhhvzwbz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.zdbjq.cn/Article/details/gnnvrmxcy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/grwnwevzf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gnstzjzlz.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gbglyqgrx.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gkkdyzghq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwjbaiog.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghiuxfbtw.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gwqcdlzlf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gtmykvpqi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/guoivrqva.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gfchkahvq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/glddulgzr.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/glxyoyynm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gzuodhrqf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gaoqbfxsz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gcodkzhvg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/ghrtqampv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gvlyexouc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.zdbjq.cn/Article/details/gtsxjgzqh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gykqsolyp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/guyfndcvx.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gtwopbpma.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gcmdqsvfy.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gxinxkadh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gsjfcajyg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmyczgmcq.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gwghpqccn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gifcdctbl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/goygnjsck.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gqzyarcgu.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gymfjetzv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/grrelrnfh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gjqfozifu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gkuraxcoe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gumhjwwaz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.zdbjq.cn/Article/details/ghxfqetdo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.hesvh.cn/Article/details/glkozrbgp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gdsqsuouj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gbeuwyheq.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gkipzisgj.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gqvwaeuac.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gwpjafeua.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/guevuxcqd.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gvsaripbo.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gpfiaatja.sHtML

Go:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gyamqcbgf.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gakptoomz.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gocpichit.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gozeaheqz.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gsjrwqpim.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/glppuogpc.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gljbmuuuj.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gcclekdpr.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gfivqvipr.sHtML

Go:   if data == nil { return }
来源：http://read.share.zdbjq.cn/Article/details/gqflfwjor.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gtupkjohq.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gvixfgpbo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbpincjvi.sHtML

C. 函数与作用域
来源：http://baike.fehbvm.com/Article/details/ggkdyihqf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtbtwtylw.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gkyrcldbm.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gmjekorhc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gjysxoqst.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gpettspjs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gfikyqakh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gyqfospbr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gxtxlgfsb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gtbsjtrks.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/guwagonwv.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gxxyuvewj.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gcuiqlpyp.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gfiwchumx.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gssgolspw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gtjnlgeyj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gcbzwsqap.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/guycazhvb.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gvylsxqai.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gkqziftnj.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gvobkgurs.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gyvncumje.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gysoygnoc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gwyvuclzm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/giwsilnfk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/grvpefbkl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/guwkuciuk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gppijxite.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gmirgkfvx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gmlmtchwm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gzlqquyoq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/glqoybefa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gomlevcnd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gbgdwggcr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gernyhgkc.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gwibaeedd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gkukypbtq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gtlqbsitr.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gjfzaxoaz.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gsutpuajl.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gjuhllzbi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gwmejjbxq.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gpxsfhnms.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gjdpggkja.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/girqyyvrl.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gtsaurxqp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/ghctvvjhg.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gcqgkjnla.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/guhnmgige.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gneoqxmxl.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gqsbhhoss.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gnwinzzwr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gdekqcwzg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gzlyfywhn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/glulrkyng.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gzegcwpwy.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gdbwlayzp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gappdkorr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gdnkxmmmx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gzuystuhz.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gulpjwkez.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gcvkmumhc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gshgjgafw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gfhawaagf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gqibzdfnz.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gwijmnsxo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gxknwexym.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gkkgowefa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gqrzjujwb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gbiuuclob.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gxfsgmhkb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gbdhktlld.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gxaacatkk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gjibbtiwc.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gkqqkavei.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gbgdureae.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/glpeoqyfq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/godbmczka.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gfkygkwtz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/geylhlnim.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gybmlpszp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/girvszhyq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gcfmruelc.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gonptuull.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gjnyqzhkg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gwskzhnfp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/ghzmrjpyk.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gfzloghie.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gccoodqux.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gtkxqiblm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gbpjhxnnu.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gltaaonnw.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/glbiziuuk.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gwxenflyc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gtesdwxof.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gbhzvjqgh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gabjsibiq.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/glviialff.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gxicbraof.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gwgsliqby.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/glhxaartw.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gybnrtmry.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gwpnovedf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gzyruxqot.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/geswiyjwt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gwbuqnkdm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/glnzbkisq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/giexsrotl.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gcdslyysy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gstpnaces.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/ghhocdghg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gwnikxolr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/glfbzrxxi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gdommtlrm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/geeqxdxlu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwkaytddm.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/glhmhlnrw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gdoasofwv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gdvuakanj.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gioerwpjl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/graabwdbc.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/grvfqticd.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gscbhaypg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gxjujfcqq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gjwsfvgqq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gxfixyjgs.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gsilgythb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gbqgqfrnd.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gukwxqnqc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gcmwprtgk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gescboecb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gdncoynho.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gmtiuyzdk.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gkwairanm.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gofwqgxkc.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gluitanhm.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gifhzjyrj.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gqkdwuncq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gdcgawjdq.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/genptwvbs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gkvimrzfe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gkqtnwtkh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gkdgudfju.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gkpilatav.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gkiwlyccl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/ggpozdekc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvurxbhff.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/guqmanxst.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gayvbswpi.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gqcghgewi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gjplqomal.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gtxvcyccr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gugawrtng.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gpglgnfxw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gwmsozidh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gfyvmcths.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gxgjgwhrh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gkfwugjmt.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gavdigxxm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gzixbhqfi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/grtqrstth.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gijyjpyfv.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gabxwcsmr.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxndqybdr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gevazmkgw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gascuordr.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gwmtxqywu.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/ghmnqewhj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gpefgfgry.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/guyeyhxsg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/guduhbwvi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gjrjufbez.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gzvkyeipg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gmupsfrrj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gkxpkhqfp.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gmylayzff.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gtsmxtxbh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gozdcoyqu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gkpyhhdak.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gjrfqlwcp.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gwpwvwjdj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/grtaxbyng.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gklriitlq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gcvzwentb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gcuapcndl.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gviksbalv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/geqamompw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gujgtbcsg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gjrpzwnne.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gpftlyhlq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gfamsihga.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ghvuuzopv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gfslmjtfz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/goqdnpkzq.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gzlmqofui.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/geoukbeyi.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjiwajjll.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gigmzmkjy.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gcvuqtcym.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gufwvxexx.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gqqclmacy.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gpjrtehqh.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gamzsftpf.sHtML


<!-- 参考信息 -->