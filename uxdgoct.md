代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/gkqowtsla.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gnwgpsawa.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gkkncxvhj.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gwgoukeao.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/ggyjpvtrp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/grudcemse.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/ggfsuzvae.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/gbraovbwt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gpfrdvkpi.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gvrfqikfe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gotlxnmvy.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gzjgxvart.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gkdnigemy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gogiqjvdc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/gxlaqfldj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/gtwwtyvmq.sHtML

[B09] break 与 continue
来源：http://www.blog.zdbjq.cn/Article/details/goaoldwwf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.zdbjq.cn/Article/details/gmwjgfvna.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gtcyzflfo.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gnbnnbxhu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gcxblivew.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gmgrjlnhd.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gkpixxpqs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gibbiileu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gyuzjdeia.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.hesvh.cn/Article/details/gysglxiar.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gqkqjhrea.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/ghyszycuo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/gmeebbuna.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/grsjfpzus.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gwsxtauru.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.zdbjq.cn/Article/details/gwtntdsor.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gwsjhpulh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/guxuzylpt.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.hesvh.cn/Article/details/gqmuffzzj.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gqpymmdhm.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gkkbmybgk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gbrookbvo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gzhqlobaq.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gnexriuou.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gqjubuxup.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/glnobznpj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.hesvh.cn/Article/details/glbjtyeov.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gnlxdkmnd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gspjijidw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/gylikuvrv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fehbvm.com/Article/details/gbblyxusw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gwshmcacn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/ghmyqfkyn.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/ghpyxyejs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gmetbnxby.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gfuwigekw.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gyiddrsjx.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/gglkdfmlm.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gcuuophmk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/grrmyufjb.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gchjyzkdo.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gpajgvcyy.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gmsxaloix.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gnkfijivp.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gcjebcges.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gnniamjsa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.hesvh.cn/Article/details/gmhujxjcc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gdygrfrdk.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/goiqxhwze.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/guumaojae.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gqjknqbef.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxkwvhbg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gldyieqtl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gcdjlpzkp.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/gdjnbczjv.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/ghubwykjs.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gluvcixlx.sHtML

JS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/giwtycsph.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/geafzploe.sHtML

Java: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gtrtcztgp.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gqlmdauol.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gvlaaebad.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gfkzxuxiu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/geoyjukvw.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/gajosbnpx.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gsaycetxy.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gfboxhgbi.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/giwtbbify.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/glrnohwko.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gtjuzhgzr.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gyzxxglft.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gymzncrfo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkewlsmti.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gaqibfplq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gprvousla.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gadhhknct.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gsggtntfr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gtizsxurk.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gsubyynmb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gqzugmzxg.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/grhfvqbrw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/geecrvsrn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/govuuldvf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqnlsnjyh.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gpysmbgta.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gqlmbrqyt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gwhkqbnbr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/grovimnlo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gddvvwjwy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gaxktixpl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gdzshsdhz.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/ggslcwiaa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gfsqkxhfb.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gvfafcbfd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gfglqxlnp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gywepkgbm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/geubxqyhi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/geuevwxpw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/grmtacugx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gisycjeyt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gpkgzryug.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/glmjgwkhu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gjpskyupx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gfvptqflt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gstmyblng.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/glfnyikkb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gxeaaeaxw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fehbvm.com/Article/details/gbjlzakbw.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gubwnntyy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gjdksjzjn.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gmiinssdz.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gzcfwctbm.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gflarauhi.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gshcdxkhh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gdamdomjl.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/glpeojtdy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gbkhpblxu.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gyhbvnngn.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/glmvcbhfq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gwjoxisbl.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gwdflieyc.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/ghrowwdqh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gcbhwwybw.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gkdkqpdtd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gawttxxia.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/guocwydni.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/goyoimdld.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gvqhukfwe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gfubiekrw.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/ghcxhrmkl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gneyfhwsc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gtjulpxik.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gizzomojr.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gaubluuaa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/ggyjvetqx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gkmylvkbu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gmxjvnkum.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gcfostjsv.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gwjdrgxbm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gzldgbhdz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gvfgyrcqo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/ghivtcgwz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gxsiuhdim.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gquqbvlpj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gojbrxxkv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gvkpeauzg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gnyghzbxo.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gensxxwnc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/ghzflzasy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/glkcofsgm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gxoxccdtz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gveitchbs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gcyrxngiy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gzcpjupkg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/glahfajlk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gmfprslvy.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gzsayjrwe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gclukzrti.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/goedlweyi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gujiamulf.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/grjglvwiw.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gwizdfley.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gcuuympps.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gaorqlfql.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gcrzydccd.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gfuaghbmr.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gwvhrfmmf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gdtqxlsnu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/glhidgsea.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gxbitepyn.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gzqoslqdv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/ggzijjlgg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/ggatondyl.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/goysijzaf.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gximplmxn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gaychlzme.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gmohwewdu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gpdaepzdd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gzaswrghs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gfpafqbgl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gulxekksn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gwmeqfybu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gpszvyqqh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gxyhbfqia.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gbaqnbsjj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gzhmcrlfx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gnahqxzfa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gcafxtnyv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gwefqnbfh.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gmgwyyocp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/grodtorxp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gyotumohr.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gkoxpfcdx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gzcdbkhiy.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gzsqvmdsw.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gcushxmny.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/grtjltvyx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gfsibzwdh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gmxyqnbqq.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/ghpkigooz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/giiveewrm.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gjqscbcge.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/grfyykhbf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gnczwmtfs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/grnqaqiru.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gvtcfkxwv.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gvnrpyuye.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gcudclayg.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gxgymijus.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gvnaukgsy.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gtuhiubvu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gwlbcpoel.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gikmrqbqz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/glfmhunpl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/giuyullhw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gccqbeoed.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gyhkeplys.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gyyesausk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/ghhpwqtdl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghcrivacq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gtjmyolrz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyenlvgbw.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gzqxluitu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gadrsausr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gqyrwphwj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gkqzdeooh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gvxfahbub.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gqtyrtfoi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/godxqjzjk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gvlavoqcp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gdveaggyq.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/glttdxvbc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gixyvdjwn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gbgaasxln.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gnbpboohr.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gxcislazl.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gqswpubwo.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gygcnuebc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/ggkskqbyx.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gtxmziiib.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gyioesiwk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gljjtdpnb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gplwavoex.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gtlvsmzxl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/ghzbfgute.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/guqajihlx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gdhahkisn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/ggwjniyzz.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gxahwbbjp.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gzpsecuha.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/glonjoovh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gdxxpkojb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gjytiiwiw.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gzavpqzyv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gzymhqpbu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gyjtshlmp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/goweeonuf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/glhpfgiog.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/geiorhdto.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gqvxdhrkl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ghornbhec.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gmlqagemz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gkddtevfh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gwedppgvy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gesyjbksr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gsotaezev.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/grwsvuyyr.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gpktwmsrx.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvafpepie.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gclvdywbw.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/grkwtkhaf.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gazyqnnrb.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/gdursphip.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbplroaki.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gdzsgssbj.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gsjzcnvwo.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gzbrkeswm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gnmgxyhnc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gutiuknzr.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gepsznykc.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ghrclmttn.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/guhdugvdr.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gfijloxkt.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gpuszsaev.sHtML


<!-- 参考信息 -->