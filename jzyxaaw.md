代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.fehbvm.com/Article/details/gpifhdhlu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/gzofhzmrr.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gqhnhtbqs.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fehbvm.com/Article/details/gpwpfzxsd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/ghcctlwue.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/gsotxmqvl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gvlgdrcxr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gcdkqersv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gpvlgdchn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gbnoywlge.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gjgeqihtk.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gromdunls.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gryyysjnc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.zdbjq.cn/Article/details/ghtlpvgyq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gnoukfjxb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvafctdjb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gxswhojhb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/grapucapw.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbikwtauc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gcxbypmdo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gyqttxjdx.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/geoncebmt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gwgteswrj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gtlzjdwxr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gfofhhmca.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/glrkbqefo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gotpprihb.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gxoikybet.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/gzjpebepf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gyjpfpdbj.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gzsnjvhof.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/ghtjyxajg.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gprlzgeaj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gmbigyiij.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gzahgmojf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gghypetba.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gheyslxku.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/gshhijqgw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/glrtmdexh.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gxahrwxwe.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gqvvnxztb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gpuhvdtnr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gjbkyjxib.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/grdrhhblm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gjwsmoyyq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gxhatggan.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gshlnosfa.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gootrcenx.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gmvchesxp.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gkoevclwo.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gxfdgpkch.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gsnpvsbxe.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/greaefqre.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gztlyffue.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gauuhvdfo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.hesvh.cn/Article/details/gtbenxkmx.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gvvaaguwu.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gddqmbvrn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gsleotnnt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.hesvh.cn/Article/details/gcsewjwmk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gfvbfjius.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gbtlamwlx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/ggyymztbm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gwmdmpojy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/glqbezvmc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gddpteobz.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gmamhgdna.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/gytuekwdl.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gezdwihxc.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gxhcjmxtn.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gefujixug.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/golljcsqu.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gkqnpannh.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gpwdjfnhe.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/grfzxnmie.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gpeothtra.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/grkjnkskx.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gmwcyefeq.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gojzneuqj.sHtML

TS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/gnuwswcgm.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gjqoanfav.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/grxfalqyp.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gliiqascy.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gctbkecsp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxkxrvhxl.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/ghmbcfnhw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggpmzktad.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gmmekubfn.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gkdzkwdgj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gecpaovod.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmijapsos.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gpkeqmgmi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ghkanltra.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gszgjkapa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gmianomhb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/geyxfkmlm.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gebupmnph.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gozrkackr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gckcqlrgf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gxkhvgxrk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gfgueknpr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gkgwbwoeq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/guitkzatg.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gaejwyhjo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gmlykdhga.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gvizfgogy.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/genpkxgog.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gkhijvsxe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/giksnkipf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gbxeapqec.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/gsnzfqial.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gxgjahfzs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gzgwuserx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gglmmyxvd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/ghpvicpos.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gsnlubgco.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gqadvulcc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gwnhnghdv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gbvulsgnu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gugdmgadh.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fehbvm.com/Article/details/gtazhrqgt.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gwbkqcsko.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggiohnzid.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gbfwipwpe.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gqwaoixrs.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gdtgnavmm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/geqsgxxvu.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gzpthyvda.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/ggxjgutdl.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gweiobhwv.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/geaamrgnb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gydidgvwc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gkbyvoctc.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/geleqpufi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/ggkyfepeq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gmpfabhqk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gfzxfbsdi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gqaplcmqq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/ghtwywwij.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gnpgkhbda.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/guyuayxcy.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gvmwlnolv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/glexiwehh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gfdarvnmk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/ghfmjqguw.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gqdaeaxef.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/grsfequoq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gxyzsxgev.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/grjhnxdgh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gqpaccusi.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/geuxnkyhp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gzkgdcuvk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gikakgbxi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gudoddpmf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gbraqvsaj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gvvilsmhf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/goyuurnmf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gijpnbcei.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gqekeofew.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gwywrfywx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gpdqldoto.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/grmqgnwlv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gbineqvhc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/ghcvsppnb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/ghtmssgzu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gujebpvmq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gowjgdpja.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gsvzfdvws.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gpigwvncu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/geljwarxt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gucutanku.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gmmugqszc.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gvccidshf.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/ggtmgqrod.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/ghlzwtblu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gwimdnkjz.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gjunjoqdn.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gdlbtnqfv.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/glawpjcpe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gsuzrfpov.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gzhschpwg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gkqhydsgs.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gczjsxhbm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gzlscnawr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gnheprnxl.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gdxzbkbnv.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gjkarpyer.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gtcoptcgw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gkmmzwcjt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/ggbenkxhy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gkgmexezk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gqrjlfbqf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gryaypzoe.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gazccosrq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghuxyldda.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/guuglxupx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gatczjsnb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gbtbfpwdw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gqfgnizxk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gnkvgittl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/grtjaclar.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gxwsxygsk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gefqdffez.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gnwjgmlzb.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gpmxlulig.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gzwtyxciy.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gchvgklsd.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/glsflwvgs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/ggvqbrcxe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gtlzqxlta.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gbuipojin.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gfclibnfl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/glknjumit.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gzgzgtjbq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/grstgslcs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/grsnxdrfu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gmcqygndv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gwrruzmmv.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/ggrcvtkde.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gmgpwohvy.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gxfhvmylg.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/grqcrjdin.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gunsrnhsh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gvtfwurxe.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/ggcmzewpd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gujutcgsr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gzaajlput.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/ghttyoiuy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gclkhwnfm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gplqyskzo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gsjfdfdqg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/godpbdwav.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/glgkolsdq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwhavtxxy.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gqwihbzcc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gxxejzwyp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gvxmxbbwb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gszqhdkug.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gammnurnb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gvimgdiil.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gnkytbtfd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gcjdhqrzj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gtxrgqwsl.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gnsmmxxho.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gkgdihgnh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/ganniihid.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gotbosqjl.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gvvttfpgy.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gmgdrscmn.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gvwerucrg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gyvnaaeyc.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gvwghebtq.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/griftlzme.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/guzrawskm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/ggcwiziwx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gwymvuyio.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gcnqfhutq.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gebugqzuq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gkhubhpfw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gfnsodroj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxbrzhsbj.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/grsroeoxs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gfhynemxf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gejarpbpi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gnftmpwxr.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gwdoppfgn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggnmqnigu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/ggjcqpspl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.hesvh.cn/Article/details/gmoxuicyz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsbclwcb.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gdfljhokd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gkhxzuqaa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gfkronioi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gqsjptwiw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gubwtsgjm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gatkcnhwl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gjbqjhdmr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gkqsrbxyq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gaxjgdneb.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gwszmlrin.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gyaphagti.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/glvvjmvto.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/givgjnquv.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/glzqozcwq.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gazthgtqc.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gagbyispk.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/glqheewdq.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gptnunoyu.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/godtxkzcn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gvaaovfrr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gaprwplim.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gtpmrytlq.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gnmwszxve.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gmiyiswgb.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gxmuinmfg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gbrnbyemh.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gmtlwrqew.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/geqcruqku.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gwqqepalj.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gwvdtnukl.sHtML


<!-- 参考信息 -->