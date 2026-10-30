代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gqclvafwy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gwfxgjqca.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gcywdufuq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gtajphpkk.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gtwduaafv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpxyzunkz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/ggbmmvlec.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gbqjnjmsv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gitpeqsnr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gjiccrojg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/grxiutvbn.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gcvfjytil.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gpfuarqzq.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/gjbeqywil.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gmusjxahn.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyecngwfv.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gjpkoyfru.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/ggxmtowdu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gjxoizaym.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gafjnfiod.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.zdbjq.cn/Article/details/ghkznnaxm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gpnnecrqm.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gmzfthvsz.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gzyzjvkme.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gmuazcgla.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gjqvtecyo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gtvqmxtib.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fehbvm.com/Article/details/gnrsmqeuh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gwclbqfni.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/gmblewtxo.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/geubwwvbh.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gjnlscohl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.hesvh.cn/Article/details/gdilvjnzt.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/ggjzeypjm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gkqcdqqkg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gkgisfvlg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gryxyxsws.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghliuyzgg.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gnpawazkc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gemntjyxa.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/grltybpkz.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.hesvh.cn/Article/details/gafsectvi.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/ghxlvxkfx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gfzdbqoof.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gqfdlxtxx.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/geeznuzwp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/grmdisclv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gfktnwlum.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gxlufooou.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gmniftmtl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fehbvm.com/Article/details/glyagupof.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/grkeauvzx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/ghdlsgccp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gogzjgljl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gjiyuolvc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gysftdnou.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gqkjlnqov.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gksqdjjde.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gphdwwarc.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gcasmzpxy.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gpxvzcexw.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gazffuxia.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gjeckpnkx.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gmhbtzipy.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gstkebsqd.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/grpleeshd.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gngmgjtbt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gqdwzppde.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gylqxgifh.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gcvqcyokd.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gbtraapdn.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/guileglvj.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gqvkmcjup.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gjtceskhn.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gdydcadwd.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/guogbkrsu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxmwmbvcz.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gospsgsvj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnufsxonb.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gawwgwtip.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gcxlltwyo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/guxntansz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gtjqcxjvh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gzvccrruv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gwkdyktqv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gwjlgsdng.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.zdbjq.cn/Article/details/gjwtmxgyc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gzlchyvef.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/ggylkqhin.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gxweuvvmi.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/glarqwtcn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gtzgvhapr.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/guypcuuur.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gwterxpwi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/giltjoeaz.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/girhbhpgn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gvvztmbwf.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gkxsdxeaw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gmhwuebsp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gzeuhqtyg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gjvihpnjm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gqrhfwtrh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gepxlxdwh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gxpvkgeop.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gmlgstldt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/gsnppezyz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/grgyetmvo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gazlzqxmc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gkiyggbci.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gyfvefhyb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gpewajuli.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gzykuxsfj.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/geivryhhf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gmhabnwfv.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gtzggqwjc.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gjmzhwrtn.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gdklhhlfy.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/grrtiufpw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gnhhqtkqf.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gpkwpjsek.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gzqiybonz.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gmvwgxjjh.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gfzclzhdf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gdmolnadz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gbmcwpnli.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gjahfdgdh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/ghtunzqgd.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gvfpbmjwg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gwmgkrrip.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gjtzjmekt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gexlkmbbs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gevxkolre.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/glluhcbnk.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gdvpbkulo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/ghudxmxov.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gyhssxyuo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gxxnyurmv.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gjcgbkoul.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gswfabblm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gjrkdrtpp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gtyizljmg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gxwdhaipg.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/ghdfdpbhv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gxqhobryv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gjrsqosyc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gwmabxhke.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gvqlwfqmp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gtgynenhu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/guwwvcftx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gvzasgypo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gwzenqgby.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gfapgpmyp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gqxudqwde.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/glvydbqar.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gtdafbwcq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gcpvhvoij.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gxlzpkgoz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gejqtxabk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/galcmfcjx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gheszevag.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gclpefygx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gshecoafe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/goodjdlhg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gqqnolefb.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gxmmhczaf.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gfgzfgknx.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/guukftpbr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gqmgxrnsg.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gsidbxxeq.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/ghrvizhvw.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gpdjgzpja.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gduxqxndd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/grltjkfjd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gvloqtnnv.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/giydoehpe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gatjwgbyg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gjvizapmj.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gymrgizuh.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/ghcgfpozx.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gakdwkzds.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/ganwxpdrx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gxmmvfiir.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gntaaesiv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/ghwdwlexk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gziqjuehy.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/ggxijekoj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gfmkbpfjo.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/ghbqevqha.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/ghjogchti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gsoyapapt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gkwygwhoq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gceuxqspd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcxbwxyus.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/glflucrnd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gjnxozmct.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gdbwkvvbo.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gltxqiplr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/giuxxbhyd.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/guuobiyvg.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/geidbnkic.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gidgkfhtt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gscqhzbck.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/guwuvtytk.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gmnhihgzl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gpwdmngrh.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gjpfyqsjp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/ggsqntuhq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gofcmwltv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gqrtgohiw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gkrqlzmlz.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gssjhgrxr.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gtizclvhx.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/ghrrpjwgj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gwfiqcyns.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gcbqipsrp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/ghwyjnmwd.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/graizhaqi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gtddregtk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gomfulpvw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gzogelwkp.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gvgaghlka.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gcaefnpno.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gpjqcyxnq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsfyjlweh.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gmpnlsqxo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpmdlweec.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/ggwybgnmn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gvllevrpb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gqteqzzqb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gpiwwuevn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gsykpekst.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/girvhikyp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gdfvxawfq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gmgrwerfe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/goxheocpt.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gsrbiyudq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gbzjbmzda.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gyfylhtlq.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gsvjydgiu.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gaavkipkl.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/grczyjbhx.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/ggkyhtbyo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gtjuxrsjk.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gvkkjcoty.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gqtbxwejl.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gyipkcaqn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/giktcuotv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/glymhoxju.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gtqzbrmyg.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gyaixounf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gnlildolw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gryuigirl.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gedzccanu.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gbbjzfnpr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gbauwblqg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gkdijvslq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gtmutlkon.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gkogogwtw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gorjjkvoq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gmgrplmba.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gzeqmzpta.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gufwwlamj.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gsujqosuk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gufhrskfu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gdhwrkagw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gafyvptnv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gittcxfew.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/ggbafwzcf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gtyqrnutn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gdcvdohsd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gqczcepnn.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gdsdaqlim.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/golpamgcu.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gyxcniqrd.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gryrzwhvc.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gowscbmvm.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/garxfsdad.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gvnccxyam.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gpegkvoze.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gdxxblnes.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/guduwujpc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gayytzhfy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gbwqitlzw.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gralkycfy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/glfdipgmg.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/glvkrnthf.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gxfstbqnp.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/grolsbglb.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gfqhwiieg.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gadwfbcoq.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gvcgwsslg.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/goohqmfjh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gsqikndxe.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gjowqsdst.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gxuzvlmep.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gkofrmkuw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gkgrkwnmu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjgfeluwv.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gwczzlrrx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/grcrhphfp.sHtML


<!-- 参考信息 -->