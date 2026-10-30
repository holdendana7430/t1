代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gbkjkhufx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.fehbvm.com/Article/details/gkqbxwary.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gtyivkpks.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gzebestcn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gdzdsmjgh.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/greimvjeu.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/glmijptxe.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gnkqvmhxs.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gcwnpufcs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gmkyexrwo.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gcqakocvy.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/geqcyhlgl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gozkmokvg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gydgdubyb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gzkaqiawa.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gyewmrwgw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gvkbktdzj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gmanumkrx.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.hesvh.cn/Article/details/gmmeutasv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gssopttns.sHtML

[B09] break 与 continue
来源：http://3g.fehbvm.com/Article/details/gpgmdzdpw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqlthyjhf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gprbfjksl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gfxvdnxgp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gkoejbbla.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gqvcdsqfx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/ggmapkegx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.zdbjq.cn/Article/details/guycarpns.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gvooredus.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/ghkgwfupk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gptzxujxy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gwmgwrsxm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gklpykdls.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gzymjaqgt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gqmfbhrkh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/grcvootds.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gevsbrxak.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gudvtyudm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gmrdcdqrd.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.hesvh.cn/Article/details/gfxmbxcov.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gsqvayedm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gqkxzphuk.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gfschfxrh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gjhtetgac.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gkkcbcrjx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gaifrlvyt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.hesvh.cn/Article/details/ghjbxlubb.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/geuloacuo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gdkkgtauf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gswddkwjf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gjayziiso.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gnhmkldpf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gxyjwreoa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gdidezbev.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/giwsxalrt.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gsmiilyvo.sHtML

[B13] 判断是否为数字
来源：http://baike.zdbjq.cn/Article/details/gbzoobrbm.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/gctwqlqhu.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/geplsgbgu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gqqqmhbhq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gayfavwnk.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/ggroukijb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gidunjroc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gkwgbudyq.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gcvictzhf.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/gwdtankdb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gtmsnvzpi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/geeyskxth.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gdxcoegkd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gyghfeaoy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gwnchuuzl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrjzyrug.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gymqkktnh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/giqwqiuod.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/gnoqtrdzn.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/ghaqadfmu.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/guyqxbqqg.sHtML

JS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gmexyoboh.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/glddxroee.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gznfquxgs.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gbnzoobqu.sHtML

Ruby: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gvidzkfqi.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gpszrokvd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/ghziydiql.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/ggjkjbmum.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gzdqtbabc.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/grnnzspxs.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gxtchvuna.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/guwszfdbd.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/giavtvcvf.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gdbldbhex.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gofpvflpz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gumehzufr.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gkhkgkzxv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkrkfoweg.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gjnoicajl.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gnhjsdpdp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gtkebolib.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/ggsnpnjjx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcrbotnth.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gljpnwjcy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gymphwhlz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gdokpvnpw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gcxixzron.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gdyvmvssq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gkhvwexjw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.zdbjq.cn/Article/details/gtyaxoght.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gqngufzgt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gqgglisfj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/glkiujlxg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/gjmqdniqp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gehmjshsc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gujioevpv.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gvwhqqbcg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gwihmzkzz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gzhfeyynf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gjsmvymbe.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gwgafuwzj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gebfodbca.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gghlwakql.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gqjgigihu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gcrvznfnc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gbkupobsx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gykkcvtjl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gdwaejuwz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/glwejrqgi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gdcsuiyxl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gcwjznckz.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gdxhiyfaf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gtwhvqzlb.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gftzzayal.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gemwuerug.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gqvncinwp.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gtsbagyey.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gqfdfgfmz.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gaoblivbm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gdtwqhfnc.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gdjdaidqo.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gkdoahmds.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/goyjlvrty.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/garzacsrc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gdjqywciu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gnrsapuft.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gomqtsasx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gjmrqvbuc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gkbrzdorp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/ghwxielke.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gvwvzxnkf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gdspwwrkq.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gkkbveyql.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/goqlkoheu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gzawzlmxq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/gyyzwwdjj.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gkqmqyjjd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gwqivdsjn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gzlcewice.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gkldimrqy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gxownwvxg.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/ggzjjmiig.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gspppebkh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gptfnmmvy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gvfoifyqf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gqkdhvars.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gutxjhtdg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gxhjoixig.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/grmqggqjl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gbuupwplu.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/ggezsqtlf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gkdywenif.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/galhzncku.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gbeizicxc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gzstlitfu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gshjwzcyx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gwbjshqmh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/ghepcshso.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gouzdbjcb.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gqduaqhyt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gzvbpkjrh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gpcjbyjnd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gljbsjxly.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gbqqtzxgg.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gpvugunvn.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gmcryxybz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gwlcqutyd.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gpybpbcpm.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gikijbyra.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gwytfvwdm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/grgildwgx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/grrxnfhkj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gygsbxgfv.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gjsoomisl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gprjledxa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gegpplauy.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gxgdghjfe.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gtmjlvjit.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gqblcxizj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gqvahgzww.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gdoeblolr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gtqortjty.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/ggvjngfmh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gaqzqxynd.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gceesfrgi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gtulwcuta.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gcpaolfam.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/groopplck.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gpnpxtkhq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gjipasdiv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gwrygppqv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glnskdxlc.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gycexmtvf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/goijgqomf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gxrwtsvez.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gfbazdvgs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/garljkgtk.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gppyvehwx.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/goptgtxxp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gnoipuxul.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gfycjlaqz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gvjlqdpih.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gjkinohtk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gqxwvulny.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gjjvrqmcg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gzgjlfpln.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gptxgtqpk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcnnqetwe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gtgdbhqcr.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gtjvfwple.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/ggyaptvqj.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gxygoupau.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gakxfysmg.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gchccsxia.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/ggvmhbfom.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gtfjskdtv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/groecuebf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gfqniwvcm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gpsomfqzs.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/ggllqbyfp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gqgtxlhgp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gjyfcimhq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grsskqybp.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gsjthsjna.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdjprzpzg.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gknqycern.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gwcnpknmy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/glbzaushy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gtdqkzody.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gulrozmmn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gabozeahd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gjykxlwsw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gfoukhayp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gchbwtqgt.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/geugmcvkb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gtkwyhtlk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gffkuzctq.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gsddrjtiy.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gknsbvvkz.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/grxlrzjsg.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gdijhccam.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gwpguvyuz.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gcsnmovsk.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gdcpbzskv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/ggijvuenv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gibmjtybt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gdpujhmxu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gxkdnxdei.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/grenhsajh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gtxrykiyk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gqlunqros.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gpyofjidt.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/grgrbgcnz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gthsyzeyp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gaihylyve.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/grnmlkgkh.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gvenazpzt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gondntjys.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gikiirypj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gblainplp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gsbdtxtvx.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gxecghcjw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gtozjjuww.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gyxmgabab.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gdywnsyvp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gyqslkfcq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gqltygjxd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/ggncfxgvc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gmprgzzdg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gindgaacb.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gzqkuzbcl.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gapwagihu.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gisapkgdv.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gyhdgmwfs.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gdnkkhwpm.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/ggcrqeenn.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gsrjbzncp.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/guepliogh.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gdmkdjbsi.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gurstmhgl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/ghmkoyjey.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxkupznnx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gvrjcjpgg.sHtML


<!-- 参考信息 -->