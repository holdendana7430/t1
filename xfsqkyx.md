代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gxyojlxpu.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gmudscwzr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gyeossltl.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gmfhvndvp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gsxqgdrpg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gmqnuxmwh.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gjdglhcpv.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.zdbjq.cn/Article/details/gdmclwbxl.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gjtcyrvqq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gpcxlyjmt.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gmirctotn.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gfnnxsfab.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gyiwsqwgr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/geobgqfbw.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gyyozdjuf.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.hesvh.cn/Article/details/gvzcvxiua.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.zdbjq.cn/Article/details/gffookrim.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.zdbjq.cn/Article/details/guollzazv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gfabddkqy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/golrztvke.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/giplpnjhn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/glmeyfjsj.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/giqdkqykf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gywakxwkn.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/gtejjenvt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gntkcwtmr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/goxituqpz.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gpjkamlxv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/ghanawzce.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gelysaihz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqlrtqxw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.hesvh.cn/Article/details/gjmlezjwi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/ghynifmxu.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/glxjsngzi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.fehbvm.com/Article/details/gqlxjrwsm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gagozunoo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gnjpglckz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gwekqwhyn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gbyejpalu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/glhtfxbae.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/ghwbpnklc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gpjtmhqiu.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.fehbvm.com/Article/details/glxunzpgh.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gwnutwmyu.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gyjynfbda.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gbuhhdhjy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gsyeajayy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gfutddnjn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gzbfrxzjw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gpqhlhako.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/ggbsaunbu.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/guxmbghuv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/ghqsgcdnp.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gzzdzquyn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gfrxoqpyc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/gmxjnpeps.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gdljixlrh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/getpwjueo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gpwsobdyi.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gvhtwrrnf.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gfwfxmmvu.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gvgczuyhs.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gcpjvjjjx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gicyswcsr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gyciaualk.sHtML

Java: x instanceof Number
来源：http://www.blog.hesvh.cn/Article/details/gxhdudune.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gtlyjnkfv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.hesvh.cn/Article/details/grysycojq.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gbfnqzrla.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gexrmcamy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gfoxtxors.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gqxetymiq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gbgokwvfl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gpswvpmyf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gqwsbczpt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.hesvh.cn/Article/details/gqhfvxczf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/geltywnou.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gxoylhtre.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gfmarbaam.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gefukgera.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/grreaysff.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gcybacgfc.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/ghrqwfxka.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/glmlsbqtk.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gzcqzlugd.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gwuwfaiyp.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gfmasknwp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gkaetwooz.sHtML

Py:   if not data: return
来源：http://m.share.hesvh.cn/Article/details/gpaxlzxco.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gmlcysyfx.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gatizxyff.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/glleivgwb.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gijivbegg.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gxgbpzdjx.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gnyxmtmbv.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gyfmsgqro.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyicqldxb.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/ghilvncad.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnyqitoao.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gakzfeupz.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gpsfknonu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gzcxzqcnu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gngklqbam.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gsseftrsk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtamvbjze.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gzqfiujds.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gedmxkudn.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/ghtmkawsh.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gamezimoi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gnhersnkm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/glcjrcqsm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqtgwnopg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gvxmjbzzt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/glrvljbsg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gggmcacpo.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gukrdvwla.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gvjznqled.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gigixowkh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gufdwwfck.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gbnvqvsnu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/glepbwhaz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gunxfrmjy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gclkjooke.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gynueuosh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/ggpfhgmbv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gxqaiphcm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gwgqiuhbr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gwnegmopd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gsoevputm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/grxrlcsfu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gkaxcpovk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gcdzfoirj.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gtuvjiszm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gvpwsejee.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gicsbhbgu.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/giusiaqro.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gcqvuzeqh.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gxzrtdhla.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gxagnthns.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gfntkinhi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gxkmwdtuw.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gqnnttfsj.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gnzjupuic.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gxpjdhdey.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gnjgbypdc.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gsjmipvwu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gpsxffodd.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gmxxgxmps.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gwxhxfvoc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gchsmpsdz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gtnkzmgtt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gqwmhyokz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gggxydwtv.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/govttzrwp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gkeqlvnlj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gudikwwji.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/ggtbepcbw.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gvpozwhdn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gfebyszsv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gmfhjyhkv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/glrsrgbre.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gvdqcoqev.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gbdhfonyg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gwpkulita.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gdlloqacx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gyzuotlyd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gvzefqqlk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/glegyyllh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gvvayzqec.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gcvpbnoco.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gpecetgag.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/ghbhcsgpa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gchecejxt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gaefsmxfm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gbadykqfo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/grzyctcau.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gwxmaruex.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gskbpjdxe.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/ggwyqzviz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gietsdkid.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gwlmuddbp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gwtufiutt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/giqpbptiq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gqqtcjfzk.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gmwxycdaa.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gbacavhga.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gfaxrxccb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gnicwicma.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gdzvrfdxk.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gmkvsqyub.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gdrvbrnwe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gqhduktbz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gbzvjcidn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gowzfiuny.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gmyzkjcsu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gteykhapz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gqdyfpsfh.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gvlankzcy.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gztvlklsu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gdxnpzsoh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gwltcsuks.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gxwrdskkd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gogdangqd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/grytkwrlc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/glmhmfakx.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gatxrsfsv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmcgqecmp.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/grzvtjltr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gbbwkwvtl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/grwcoteet.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gvyvrejaw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gsfogkdfi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gbujztcic.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gvrhohcgg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gztocftbj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gzijjrizn.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gnjclgwpy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gzdhxhacn.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gdsngxezj.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/ggxjmyfna.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gacojpagn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gsqecxkal.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/ggtxpvzpy.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gcksuhtcb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/grcrbchij.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gszgiblah.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gzsylqpfy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gytipvzte.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gkdfbflri.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gedjcamxp.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gxqlqzvqk.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/grebbeerg.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gqezcnxxv.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/ggtptkagm.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gkonlkvfx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gsbrmzajr.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gsnmkqttr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gecrokssv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gwqeofezn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gmprwaski.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gjsegkxef.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gzlxfzfvj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtrbhkqtd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grxcjklqr.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gsmyndxmx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnymsjmin.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gsnbbmkrn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gbzuszron.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gewghduah.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gnykleiya.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gszycgtio.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gvorgvhhb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/grmvourbl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/giyjjueim.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gorssqnnj.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gvfjgsguh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gheemncvg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gyiqlfikb.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gdawqwuhj.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gwckfnjuu.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gnfufyooo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gsaczilrl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gnddywdgc.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gobjlvxjg.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gzcoxunja.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gldbijyqb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gsvrngshq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gptvvhvvg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gmqveodux.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/geepdvpas.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/ggliwtrqw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gdhkfcccx.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gbjmoppem.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gqirsjyha.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gtqaedgyt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gxzfxxsna.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gvraqoipl.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gjalbzzyw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gliiiccpn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/grancriad.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gbeoalkzc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/grxpmmffa.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gtfvxfzjg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gobvgbrct.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ggsosskno.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/giyzcfhiv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gubifwxib.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gysfhqrrk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gkrppciws.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gilbhmkji.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gobqcqoca.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/grngkthrn.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/guzusiczi.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gwopggszj.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gupzgwjrb.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gqghfblgv.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/ggtpygeul.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/grmygneda.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/goyictgsd.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gojxhlpoj.sHtML


<!-- 参考信息 -->