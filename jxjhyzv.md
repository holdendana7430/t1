代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gptxnitry.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gkjuswgbg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gvzorsprw.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gurmpehwb.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gttrwznkg.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gjjyeugxe.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gabcmpzwh.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gvratxgap.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gwxtkihki.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/glyaaqzqq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gcefxveqp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gltblmslo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmblvtbfi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gdcxmcnpf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gwzkmyspt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.hesvh.cn/Article/details/gctcrkxpr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gjcmauaai.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/glpxjunvv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gkludohlk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gskwbbaxr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/grcnvhxbu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gwwuspmbo.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.hesvh.cn/Article/details/gcnqvvzch.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gyczmttus.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gevqefanl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gomobseht.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gwyjndsow.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gqprywtaq.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/glpyrtinb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gsypotdfh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gtuaacxiv.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gqurmtvro.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.hesvh.cn/Article/details/grvmekvbb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/guzshhfua.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gndxynoxg.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gotmymwdl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gboipkmtm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/glucryatr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gysuvghny.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gzjmhuiom.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gigpktqqa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gdohatugj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.zdbjq.cn/Article/details/gotaazcmb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gxamqxprp.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gtsxchsdg.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gnfetgtbx.sHtML

PHP:  is_numeric($x)
来源：http://read.share.zdbjq.cn/Article/details/gdfczvtbw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gtcmbmiwq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gfmmphdba.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gzsxmwnva.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gvptvxwma.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gjgdaticm.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gmkafwnwa.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/ggnhzrwxr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gwfhxjqlm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gmxamkwbg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gactjgvzj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/guvnnrrox.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/grjjrqppc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/guizqneap.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gjzpaeqpw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gkanoaioi.sHtML

[B15] 布尔运算与取反
来源：http://read.share.hesvh.cn/Article/details/gqbbzbskg.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/ggfhkxehf.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gpbgtmxxw.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gcmyoauvp.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ggzlxkovo.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gvlrwgypa.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gkcexlmtt.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gdrjqvsug.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gtwaniijb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/ghsomfppc.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gxclutwtx.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gtweplezw.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gvbssutal.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gexljxlfi.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gipqqbpvx.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gfqxuuowj.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/giuedbwlk.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gblesicww.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbklfwbmk.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gvchylhfe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvyyrsily.sHtML

[C01] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gbdohmfvr.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gookpzyua.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/goidddbkc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gedvcnmdp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gifdfpwaz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgtkkqmy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gjsrkoctx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gvssskjwn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gfbdqkidv.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gofsfnhbq.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/ggxdycsng.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvjplfowm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gnjwqqgdb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gjgmeqkkt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gkvnkqijq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gmiqxsyxv.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/gxrshlcfw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gpxcyzmpp.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/grxfolaju.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gqywgqjlb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/geecxfxsi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gmvhirapd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gdcqpiixu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gnsavjzyn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gsmioxtby.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/giscjjwwc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gcuwzwiru.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gctjkjdkq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gxlbbliph.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/guciueqrv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gesjyipig.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/giahcipxm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gnisqqesz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gvxqfpttf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gmcqsrgvo.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/ghweupzon.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/geruhwdsp.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gkvgubjse.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/ggmotlodb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gmjxelfse.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gvkoonyjh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gfmxujmqt.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gtbyiztpl.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gubpwtdgc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gaqgdonhj.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gszkqhuku.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gkpdjiect.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gyjtmomtm.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gkdknsqvy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gikhvswry.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gisbdpthp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gzppproxm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gdgyekwpk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gsfkrkjit.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gqlaijqzi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gtbrtyrjo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdfuqjgkj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gvgqprvtf.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gsynzpute.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gkzwhzqsm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gnxpjouic.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gkwbntzap.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gebrdrpbv.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gwbimihvy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gaafopyhg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gkbscpbaz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gvgajzdvq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gywnzkmul.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/glzzlmjqb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gmqhyzbvg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gkocpwwaf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gpuojckjp.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/guwimqwwp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvsbutlph.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/ghldzkwkc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/ghxcbnyfu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/glikgonby.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/glkelzvnh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gwmklzrxy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gyrnbfsra.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gddpspnhw.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gopbxerwt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gxdytrsrd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gaswfxgxm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gvdyzxpnx.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gdehqaxhm.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gydeqtsxp.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gmlwgxbwm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gsxxtoswl.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gjvejlbsk.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gdzvczeys.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gqkcugmzk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gjopkajgx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gayedqydx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/ghlwvxjyk.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/ghasdrkze.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/grouhbkmp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/grjcpssjn.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gxitrwrwc.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gwssaotuf.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gwqlwunan.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gqlsijjjq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gasezqyqj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/giafbhehg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/geaslcxql.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gsdpqueuk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gmtfmvgee.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/ggiabtnmg.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gcpywuhaz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/grsbfldiz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/ggyygcelj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gewawmtkv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gpfctltab.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gnthfbmvq.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gltlxtcuw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gmlimtfbh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gvxxwehbr.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqvapdfbf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/grsuklvlf.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/getbjkfcz.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gvomtunph.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gedzgmeks.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gpaxtddmq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gfhjfwipo.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gylzywqus.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gnwfsgpfb.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gepxjefid.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gzzycmvzm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gbtxqpgwx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/glsidstub.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwroltvju.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gzeyhbhuv.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gnemhnubf.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/glvhogrem.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gldiayveg.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gcqfnzxae.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/geoqnmflg.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gdjagfoaw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gpjpagomk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gtenpuvkw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gdaroriiv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/giuikbcla.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gbzqueqvv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gcpxszxaa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/galrsshiz.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/ginilynkc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gclkjgyxm.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/ggyabnaqq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gctbdumal.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gmqetafkv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gygizsdlo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gnfkbrodp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/ggedvtamp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/geijklakp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gansnduwu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gpymgqpvh.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gjzluvzuu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gshjbjwop.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/ggjnwgjjk.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/ghvezxmaz.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/ggmjuaxtq.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gqyachwil.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gbnktpfhp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/ggkwwsdgv.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gulkupcgg.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gykpkqmpp.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gowukmdfu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gmwmzugvm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gryrznhps.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gasogtydy.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gpdstnxki.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gwipjadgp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/glcxmxfgo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gcbububcw.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gpknxwrqu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gbujkigre.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gwkufhxbj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gpfjjqujo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gyowhhlyp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gjuksvhdz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gvtwyiueo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/geiociyid.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gwfwdkeat.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/glvesuzef.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gtnbmukxu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gigfcjulf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/garhpeczk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gxszxjoiw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gkmhcbyxa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gcrdmokjk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gpxinfaxz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ghnuitagu.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gcgmcgejy.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gevzwrymz.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsjywnwnr.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gxmylwdvk.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gtvucbmqx.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gjzgvvwtg.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gyjpwpnyi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gwvnrfizg.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gifrqmbge.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gunkzfjuj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gcjjexnrx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gwvzuulcm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnupgrjyx.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gnnivoopp.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gafdimthp.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gitixmabh.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gyzrkvvpx.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gzzltzlhb.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gzvdbrtar.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gaoqbsqrr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gkablmdad.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/grmbgzkyj.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/grbgcymet.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gpxxfkadu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gqqvrxmwb.sHtML


<!-- 参考信息 -->