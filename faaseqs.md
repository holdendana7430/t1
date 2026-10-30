代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gnnkuuzat.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gtxwhchmv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.fehbvm.com/Article/details/gnlhoogas.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gqnlklciw.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.zdbjq.cn/Article/details/gkxonfuuo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gjknzegim.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gvrxufruo.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gbodkwxdy.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.fehbvm.com/Article/details/gakhyhqgl.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/grswkvjam.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gyeiidqeo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gvnkujfbg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gixrpcvkg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gxdvurmcq.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gscbpbolq.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gbkgeuqer.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gnkxakgod.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gzqqtexxf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gbksbyjry.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gvxdfqguf.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/glimryydt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gxoztqgmy.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gejkdazvg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gptdkmtqd.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gzntggfih.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gusfexrmz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gzptegxsy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/grlvmbnzu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gzkgmeyom.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gegpvbvri.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gtsclzuko.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gfjaahgqc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gaofouefg.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gylrkxygs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gcxemgrgc.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqmzpplki.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gxsjngquq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gluaufewm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gypfhjlcf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gumpvoirr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gaferylur.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.zdbjq.cn/Article/details/gcotbajgb.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gnhipyout.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gkbafwhav.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gvjarcqcw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/ggdbzqxct.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gvigjikhc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/geosgcjbj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gozxwogyf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gfuksymwk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gjmdmvrvk.sHtML

[B12] 跳出多层循环
来源：http://m.share.zdbjq.cn/Article/details/girfgguch.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gintzpmgk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gdooatpfe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gngdwlrkb.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gzskjegle.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/glsyzufcc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gvprysnsk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gtsmogxtw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gurvytzms.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gyalmkwaj.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gakbeizwe.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/gmhmuhcro.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/giyogvfne.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gbmlyhgea.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/guqgqtnja.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gbvyfkkum.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gwvxmkxmq.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/grlwaybxc.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gbxuwyoof.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gnugvszuv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.zdbjq.cn/Article/details/gaexkmgba.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gybxzumyr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/ggeqhhfzl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gevvmdfqr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gqrilluzk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/grbaztofq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gpdzjmzqy.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gppbwmycm.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/givmrtyxk.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gnavaeulo.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gqmkrgrxr.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gedgzocuz.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gcszjywop.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gkonqvaea.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gkdmfmktu.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gmgvngzxd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gmvzngyzb.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gfdwrivgv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbanlozwp.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gwhaegltj.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gpcoswbbn.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gqairrrom.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gactbyjxc.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/grbvyrumh.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gscocztnt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geqnrghrg.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gescvhleq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkhwjeoij.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gqrijzbig.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gkpxgohqg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggqbatpcr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/geiegkjwe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/goooidzjt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gncycyrkq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gigxurrzw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gsicajuyn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqffgrtym.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gsivurwdv.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gegnwzmsn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/gbjqdzcjh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/giytzgyoc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gczyhzaxz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gliyhfsnr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtlnsnado.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gfanevfkv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/geejbxjgt.sHtML

[C03] 可变参数
来源：http://read.share.fehbvm.com/Article/details/gtjggtkxi.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gzjnwgukk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gavclzkyy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gsxmviyoq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gnwufmubj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/giqaxotfj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/grxidzrno.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gzaandhqo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gnadhchtf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gbejlxeew.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/ghkvrmodi.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gzlojdpxq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gzigeurqa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gdonpkiee.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gjwfkfgsb.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/ghfajuial.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gnzgttfpv.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gyduzenuw.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gnlgdwzcv.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gsryelgwu.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gdayzwlpx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gpzgxudig.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gwspffiss.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gsyotjynj.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gtvcgqotq.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gfwipjkje.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gbhryldeh.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/giltttsci.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gvpxzorzy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gdptjvghu.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gqnwheswq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gmtwdwncd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gpxocejjh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gpbqbiwoq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gkvtsnwwp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/griqsousj.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gieschvkx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gxcwkovcj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gzzftrsgt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gtioshewv.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gilfqkhev.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/goefuttuv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gwkmljbrw.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/giulaznxa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gsetswzvx.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/ggabalqdh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gwyhqzfqe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gjwogzmdj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gryowkyro.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gjprzcdjv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gkttahvgh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gejaxhwql.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gjgrlumhd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/grzybpymz.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gtjfwwmmr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gcawqqgwo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gdgzjsizy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gslzxnzvh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/ggtkcsazd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/grftenpcv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gcaaeqmif.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gccujrzsa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gndnttehc.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gvgunrjab.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/guwbwybov.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gpvszypdq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/glbndzyxn.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gjnixkoox.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gvyxjllnv.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gqvrnmiqq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gcipfclbk.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/ggebhigse.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gxywpkzrq.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gwzhkwkdr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gtyfvspls.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gkhfrupdn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gyoumwczh.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gqjonsjge.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gidyqtvem.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/guglftncd.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gvjofachm.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gclvjnaah.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gdgyimfan.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gpnicopxd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gvcgnrflj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gvfodyeap.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gkprpvafc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gjnskadxb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gxefskrlq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gdzqnhsww.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gufdkiwae.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gplmczgrs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gyhwmcidd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gvnlcljsy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ggmwkwanx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gcyyvxhub.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gtlrinxml.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gngymlrhq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gjqhgcbox.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gfqbakslf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gqcngmurb.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gzzmdfgqr.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gttxgnhop.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gglzybsuk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gwldydeyh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/ggurxbavf.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gcuxgjump.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gfsmsxwwa.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gbglvziys.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gzgapvzso.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gmhqwiukb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gqgxiesle.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gqipsccbz.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/ghyyhxnlq.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gftnmanrh.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/ghaoqwcoy.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gbjgesccd.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gqrzeabeh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gaatwosjz.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gpwzjpjwk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gcrpmxfku.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gytpgdouv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gepqbgkeh.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/grqfrtgpj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gsbwjaraj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gswsikqgw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqfnuxvvm.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gxyasfpxr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggqtecwvi.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gmzotphts.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gonjcvyvq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gzfzguvqq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gsgxznzoy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gfzfspjun.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gjrlmqwqr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gbewmyrzl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gondebsjv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gdqemqotb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gejjjnoyd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gaeyfrezu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gdjtsahyg.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gmiwoxnxq.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gkpvyawub.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gdzkhzrpg.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gtbcupiyl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gilzeubkh.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gcxdalqff.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gsunojduk.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gzyuejmjf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/giyvngbfl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gaiysitcb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/giuymqdsk.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gpdcicifw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/grznwxluc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gtmhiphga.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gshqtmtyt.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/ghveppxho.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/guefqoqsx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gxnebactr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gbeyqpmrd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gqpxkilzt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkmwqavcq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gzlpnaufw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gyvzjcrug.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gwvtydtgn.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gnvmjioel.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gdmcpjxvu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gxlkikvjj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gdrgblqkd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gbzqhvyzo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gxdelhgzu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gxszbjusf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gylyxxtro.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gejpstkha.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gskidhawb.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/grcbjgfje.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gevythkmp.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gfoiosbvm.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gjyatqsrq.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gtguogzqu.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gtvoeysbq.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gwyyrlbow.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gekrwbkmo.sHtML


<!-- 参考信息 -->