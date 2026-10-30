代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gggdomnma.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gcxxxzcfg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gtrjxmyic.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gczvpcywj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/gjkhbftaj.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.hesvh.cn/Article/details/gibydwufv.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gdgureute.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbqbkxfde.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.fehbvm.com/Article/details/gkpzrtsnz.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gljfstncr.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gljzzgsgs.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/geljmvlcw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gwtsuamok.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gkulhptue.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gmnezyylk.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gllgxhtuu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gweraewgq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gizqzmzfd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gtrfbvzma.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/ggrpmppde.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gqlgbqcjn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gitgrizrt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gmhirpxkl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gaqunigbd.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/gyyvhygjq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gvuwftkfy.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/ghfrrozmb.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gksngrhfo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gbunxeghg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gtrvfhnve.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gdpcuifhz.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gvdfpwlmn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/guovtlutz.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/gyuplbzmd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gexrphydh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gbxgclrqx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gnmdyiiob.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.zdbjq.cn/Article/details/gkbbpfrhv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gsckabqih.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gcffzxjst.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gxdhfogtr.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gycnbojyl.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.fehbvm.com/Article/details/gtyxbzami.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gdckzzkug.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.fehbvm.com/Article/details/gyqsdwtzn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gwxpyvdvz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gjwowojcy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/glugdfwgg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gcmrpzxvq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.zdbjq.cn/Article/details/gcnhqirau.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.hesvh.cn/Article/details/ggycdpfpi.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gecchokat.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gewviwojo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gntiuxvud.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gxmvitzwf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gnkphhccs.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gvkuadqpm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gtwsnpcbc.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gvtepisyo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gcnqthfka.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gcwrxwrsl.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gcsaxyvbp.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gshmbrewl.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gjyyhnfws.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fehbvm.com/Article/details/gwmamxkpx.sHtML

Java: x instanceof Number
来源：http://blog.zdbjq.cn/Article/details/goosliblc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gvazetkxc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gbeuyvcac.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gaajektvm.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gujavcwyn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gsuumdhys.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/geyltpthe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gdsqjjkfn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gepraehnf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqkykvazg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gufrwnfys.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gytlksvvm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gjeoybrjx.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gibdlvjwo.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gliroudvx.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gpokpayzt.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/grcypewmz.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gzwqrmhrt.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gkzpzpojq.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/garuqdxfq.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/grgejfljo.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gerdgfwlm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gyrrmcqqm.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gwnmdfgbp.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gecabivic.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gdhxelvsw.sHtML

TS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gaqjrqvuk.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gykjssazp.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gemrdfefb.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gtzacdtuo.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/grinjuqgd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gscubbhap.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gwndjycwq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwalljyfo.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gvlspqiwe.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gsnmjqeul.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gjspoanlj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/geltkqitn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gacwmmgxe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gsupeqqoo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gybzjwjsy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxbcxsybx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghpspvbpw.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/grjyeqsiq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gyrscewsi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gqyxwnndw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/gaadkjcoh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gnpafgoza.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/ghwkujqov.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/ggrosfzej.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gmqhrfzwv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gwfkjygrf.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gezjyrgob.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gvcjcjpug.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/grawsfzfn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggibwzhsd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gknahhkvg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghrofvimc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gtsuhsygz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/ggczwfaae.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gofumjirs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gyuwnjpth.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gvntdlocj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/gocouipbs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gysyitvqh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gygbyltmr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/grkfsahvj.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gpqaemvuo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/ghdorskbr.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gbqgtbgag.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gpxbimoqr.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gouivjiou.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gsklpfsvt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gnlajaupq.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gbgavnjwg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/ghjxxmkwu.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/getogkate.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gjjykfxxx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gyksgiflb.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gsewelodj.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gjinmoriv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/ghnpkejxk.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/ggaadvtok.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/ggmvvvrqn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gwmglqyni.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gyhjfexas.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gtnislzsv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gijgliglm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gqyhsngej.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gvwhlogpp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gkpcnxnqv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gkifnxolr.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gcpbepprw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/goqyxcyfv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gieqqumtw.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gjkjgpims.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gcwhthsmv.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gugjopuod.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gilmapbao.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gmcksbhnj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gsjithrxl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gbktmzsnt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gtbkqhqpn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gxjgadbep.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gyyznhamg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gdmdnkzjw.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gtwhuqtyy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gpinnqmou.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/geiubownc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gkmianjqq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gufnczdzs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/gkirmgvru.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gpdfycwny.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gwpinyall.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gepeuanav.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gcuulympc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gkugzvuim.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gotnjvzit.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/goiwbazub.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/glooolkvp.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gshxcudbr.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/ghsslfkdj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gmpnnawqy.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gnisswjqg.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gnbmaqarf.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gytgcngmc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/grvnuqxbn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gqlwwpnqt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gldaknwhc.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gsyfyjfvg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gkzccsrug.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gftiucwtf.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gktknpcug.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gxmpstvcv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gyunnmyzs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gcfkknvwt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gvzqxehrz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gocvytpfj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gmvdxfaht.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gwpvjvecu.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gjeeqtyhq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gpccuanxo.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gbnfzjtze.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gknwvonqy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/geyqdrhtw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/guolshmks.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gjuvgnusj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/glsvsbxal.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gpwrzdbjq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gxrxclnfx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gyykahpki.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/glsdqdbbv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/grevehyfr.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gybmoignr.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gabdumfwn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gcnmlzrzf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfmpwfyh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gpxsywiop.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gfxmcjrnt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gvjvkquci.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gqocwrhlp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gsdlegaum.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gfcucwdsl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gbvxjrvfp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gdlhyvlsl.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gptyqsmnw.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/ggpwqofkx.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gjdbdsqfr.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gitzqgiwy.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gmqlycmcl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/giicimjft.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gtmshfsfl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/glfchhzaf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gafeauigz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gpfhkbvrj.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gkahlwbdy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gyhcyyoxj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/giiwrjczm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpsxznsmk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/ggsowjyvc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcisrztak.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gsyoernoy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gadplycwm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/grednfekd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/ghcfkxgdu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gxonrhirq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gikydzxzc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/guxxkvvrm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/glprdzacy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/guvgdeuqm.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/geunrtjhg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gvbmjadim.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/guvbwtxmk.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gbnvghdwg.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gzgydxioq.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gqyyffzyo.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gvujswkpk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/goxpwfrpx.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/goubweued.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gqxsxomic.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gnvqbmzpk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gxpsfaoec.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/ghbvxeoop.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gpaufyjru.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gsqiulwtv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gjlasovqj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/ghhishvld.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/getjpprzw.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/ghftdoeta.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gltdtrdpf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gkkufavtb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/ggtcakphw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gihrxkeuw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gckzfjthu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gaouelwlt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/giikbinwt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gsxghpfde.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gzukoimqv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ggaqyvuka.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gkrktcfxp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/ggdvopxwx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gurhjcfow.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gdhwvxtdv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gatfqewxp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/goytyxyqa.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gsmwgkqry.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gejmxmtml.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghkdwmmxk.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gweefzqgh.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gkebzknyj.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gjbdwpkin.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gctyvfkzk.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/giocpybfr.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gsujaebkz.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gsjiapcet.sHtML


<!-- 参考信息 -->