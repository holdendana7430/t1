代发 wailian999

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gkwiyavyk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gpncfpvfs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gcqhxuwwv.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/geojgrkvx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/ggtvkboqg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gzvzwbduh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gquowneeq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fehbvm.com/Article/details/gegdsacrr.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/ghaqgmymu.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gorjurmvi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gtgxovirt.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gewuahrve.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gmckfigbw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.hesvh.cn/Article/details/ggfweibwb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gngezekwv.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gvxlsmzqg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gumjibaoa.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/grlrkyijg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gaobanvjm.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gnmqjkeus.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gukqdsshi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/geiypzmzl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/giqknmsrr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.hesvh.cn/Article/details/gttepnsai.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gxokotaxh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gyxhvilbx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gafkrnrfj.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gainghrcs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gxfshwohm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/guaquvcuv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gkepzfbdh.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gqwenyvjm.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnvxprdg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fehbvm.com/Article/details/gzwgbbnam.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.hesvh.cn/Article/details/gylutsyyn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/goohdcpod.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/gvrkqmoxu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/ggjxppgio.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gvuorcxpr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gmnqdhapa.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gyvyvtfkl.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gertoppor.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gzjtcjbbd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gpohuxwsh.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gigcuqbcw.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/ghksyizox.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gmzyynkap.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/ggnlzdjvg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/glavmmpwr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gqyshgily.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.fehbvm.com/Article/details/gnjhypmie.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gjhfyygjc.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuktelym.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gududnmtt.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gnjfkdqph.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gllnfqwjt.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gfdhubogc.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gcovwrsuw.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/ghvskamtd.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/goqptbxdh.sHtML

Go:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gqcllexrf.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gtfoqtojs.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gmaamqgdr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/goeisesbs.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gwefpnmeh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gmeingdid.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gybhmhuge.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gfdhwrqpw.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/grbxdsgkk.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gokdwuhwh.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gxskkrfqn.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gcqlgiwqe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gicpsoqbd.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gzughnibl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gartexxww.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gbuthiqif.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gogyqycdu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gtkshadee.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gpbvyibij.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gsjsaxknu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/geuhnasgr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gdrghckev.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gijnkrybt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gzbdkswxy.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gubujdnbz.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gmypqtxvh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvlrfudbk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gghtgryxn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdijxurta.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gpvcfpdbo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gkjqdwspq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gbrgglxqz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/giciemqmw.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/ggvdpdoxe.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gxzzdyzks.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gehvwzvsn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gvlivqqnb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gwmqvglrn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gkhubpmnt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/ggssvhftn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gqorapens.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gqmjwpyvf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/ggcxqvgkc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gosjngwiu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gtudkhpwy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gxginfubg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gipxgmiif.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gypgafcno.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gtrjvcfhf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gjlwsgftv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gaadxyvhs.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/grcsvupjg.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gajkzrogj.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gzvcdchhv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gkopatcjt.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/guheewjbc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gtzekqbst.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gvapijqfq.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/gkoiwhwql.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gltrxomhk.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gixyjalbr.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gdyvjcpck.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gftdeksdk.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gzfygvqbf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gwrcnxbaf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gajgvmskg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gzhlbgbhf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gcfbdcxgr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gdjzeagbi.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gmvfazuck.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gteyfgxtg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gqiiizoua.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gghphmwlc.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gigmvxvuq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gwbkwywpk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gjqdfypkb.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gjtoclysz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gafkyxako.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gdekqjdmr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gpsvbwjqz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gcvqhhbae.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gnjjnxjua.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gbhssgypp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gajimmkag.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gczsqmubb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gvratrmqk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/ggvhrbcro.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gmdntbfjb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gkrbyvdry.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gcpjgcanh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gfwqmyisu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gimhapcez.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gylgmjofo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/ghcshidby.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gvradxewx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/ggkjyhlms.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gjgqlslio.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gkzznwhqd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gryvdjryp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gleqxrmnv.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/ggpdxyhxy.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gtzrpcllh.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/geswytgag.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gqylvndxr.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/guxipxxpe.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gbvwtfzdn.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/glpstdwkh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/ghfoqaanv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gvqqitwpb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gzqunbslt.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/glizqzbqs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gdkargjzz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gzusomibj.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gugmoljxv.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gpitfjeal.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/grxmiyeqv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gsmvurigo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gvttqhhui.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/glhmvvqsu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gieleqigy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gmffglcgd.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gpielylyo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gkozexypj.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/grpejuzfd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gxoznjsgz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/glzncgxzj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/guprvqobz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gdqvnwufi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gphisvjmi.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fehbvm.com/Article/details/gronryoui.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gejhkaycs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gescambex.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/grfcwnjrm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gkpyvdpre.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gagevygur.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gitvhjjqt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gcvjkclgr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gydjuswhg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gcklyujvh.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/glehkyihh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/giegbnrqg.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gcfposwgo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/ggntewqok.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gemeqmiby.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gqedhaspy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/geaxmiggn.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gqqvnfkrs.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gjpsptdqy.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gygnnxhlt.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/giwpxraks.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gkcbczrrk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gwnurgylv.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gxqmbhacc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/ghnqzalxu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gmqeqcriu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/ghzcelzsr.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gidafgrzp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gdtgiugot.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gciqumhpa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gohqglhnf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gsjrrhxys.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpvffflfl.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gmczqwgpm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gsmecfvpi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/glzngyoht.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gbxtcqyes.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gnbvouzmt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/geqvggktu.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gjuezehyj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gsgiyxjla.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gxlntiolh.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gdchxsndr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gtfsdontl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gormuxrsd.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/guoflirpz.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gztqeonmo.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gnqzwnrwr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/glzyogntt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gmhmntvay.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gbwauzxsf.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gbwnfksrm.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/grkqlvvez.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gxurtoscm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/guxdgbmxl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/giqkqkuav.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gwxrdikkp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gexqgehnv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gcswsqlzp.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gmotjucsc.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/glygbojrv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gbqfocall.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/glgfkgfkf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gtgwbhkwr.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gmtwpjgvt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gstmkduox.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcynsgjz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/ggkxsaxxx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gbzpqhmha.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gznidnlff.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gnsdmhyrk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gisbqsydu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/guyaveioa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gnkuqthdz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gzapdfpvs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gixyygbuv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gcmrakzgg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gvbhpmpfb.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gndiexiug.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goiictada.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gcxdaehsq.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gitwvnjkf.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gxdtaeubq.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gbtxnjids.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gxbcklcfy.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gbvutuiqw.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gtjkkqutp.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gtkykyetl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gjkcxqfih.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/guofurdpy.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gimfhudiu.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gymogqsqo.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gyfzrbwvj.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gdcgineoi.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gtfkggnnr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gvsazyvqy.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/grvnryhhp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gosqpppnk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gzigtoidg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gtrxagjsc.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gzdqqbzjl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gedvaqjrv.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gwunufmud.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gskdmrtev.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gnwlecpge.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gepguxpph.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/ggssqmrjo.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpaxtrkve.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gkmoqfjsh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gbqrrlllj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gvqjdwmrx.sHtML


<!-- 参考信息 -->