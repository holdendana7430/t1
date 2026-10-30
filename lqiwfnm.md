代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/gbeqzlfkq.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gcnpjakpw.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gyfzxngyo.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gpwxlgqoo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.share.fehbvm.com/Article/details/grzwqhsvj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.hesvh.cn/Article/details/gjzwsokum.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/giuskwemw.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gneokvekl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gatbpipmz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://wap.zdbjq.cn/Article/details/gmpusdkxc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gzjwuirrz.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gnawyoxlt.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gdzahfdpf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gaukdysbz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gzndpzuwy.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gdseeqcqb.sHtML

[B09] break 与 continue
来源：http://www.blog.fehbvm.com/Article/details/gyevidtru.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gbnmymumx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/grqjluzyr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gvdogknfm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gkbryzbfx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gixutdaqx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gxrrxxhhq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gmhmqmqcn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gnzqqaboq.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gpnaexzxs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gzdejkbfv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/ghraishtg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gqwaokjku.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/ggurzamub.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gwddgktvr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/goejffbvp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gtdinptaq.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.fehbvm.com/Article/details/gysrxbvfc.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gfgfzekil.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gfzogvqup.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.hesvh.cn/Article/details/gyayazbme.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gttwblcnc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/ggcfuxdhz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gtomueolg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/ghzmicxaj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gapohdble.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gnaifijgv.sHtML

[B12] 跳出多层循环
来源：http://baike.hesvh.cn/Article/details/gzizfzjhm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.hesvh.cn/Article/details/gelztijag.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gcgdpnpge.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gfvjiumet.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gshleawtc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gulobtbfc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gmbfvwqtj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gqsmneusx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gbfiqwbvt.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/gqyzrmjuo.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gfbvegscw.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gnhzsubuz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gvzbbpkzc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gpzoxpvuh.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gitbflddt.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.fehbvm.com/Article/details/gdjjunzei.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gjaubmgxc.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/grorrsfme.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/gthrwrdss.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.fehbvm.com/Article/details/gdyvlurhs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gfdvkyfar.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gaqkzaxly.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gkhjykrnl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/gvmiufcdk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gnbulvkou.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnepqvlur.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gqflwxhyt.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/ggsnhhquy.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gewthjbqg.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gfqkyayrw.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gvpxhzbwa.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/giojzhfob.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/grrawtpbh.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gstdcezcb.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gvrusfhcp.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gspmapgbl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gpxgwqzjc.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gllzzzcsr.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gplgdsbos.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/grbedwgyz.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gljaufclh.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gdvwlepwp.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/guitonspb.sHtML

Ruby: return if data.nil?
来源：http://baike.zdbjq.cn/Article/details/ghueaczyx.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gdwuonzki.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggdlfvpnz.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gtuwtpxdy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnkniduwy.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/glnmlgemx.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gsqnqbcgk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/ggxyjpvkj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gnmcjnfqu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gnkdeprqz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gcflnbdpg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gaktjeiul.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gpxhpzvhy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/glbslhynx.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gexnmburx.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/geeflwgvc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/glsmntjmi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gyggrzbky.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gugbyosxf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gsdhnnysd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gabccumjw.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gimkqsmom.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/grinqhbnn.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gwokuoyzh.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gnwkqgpjc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/guucbveqd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/ghjxzcriu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/ggttzeztn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/grcfsagbr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gukgvlrev.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/glqxeaesh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gdxqakhds.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gmdyxeaat.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gxnfsrbdm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/grvqqlazv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/ghxxkwxpd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/grmsogciy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/guxbpzitm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gzszvqlsy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/glgrnbult.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gimixnlrx.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gpkpdzkcy.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/ghlgapfvf.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gtaibzodg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gqqnycbnl.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gicwlugsl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/goyqvfuhj.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gljgfuqav.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gzszibxdd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gzhrsqxqc.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/ggywkzjfm.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/giziaiwgd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gzshiwnob.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gokxiznwt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gudoibeha.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gtrubcaey.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/ghwkimvyq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gxumnpzkl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gqicwkqxd.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gljsbfazl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gsyhjfdxx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gflxfchvn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/grgwlvnne.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gunuujyeg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/grpjoihrq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gvccinaky.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gnpazujqv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gaapphhse.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/grrkmapfq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gsmwlfrnl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gaayscopl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gptrzcrfq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gpzauisij.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gjbazgaxp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gqemwrajp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gltstshsc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gzluosfqu.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/govpaauad.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gwywcezbr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gwninvzfw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gsgjvzjmb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gkqwobzcq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gheqsyjze.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gegjodshw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gjttdomos.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/ghdjouusb.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/ghfvwbcxf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gbdkoubmq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gixckvspn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gjzmabxwj.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gdpdnatah.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gbrialkuy.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gfdkveoei.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gfdntovpu.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gsqfojwuo.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gopiknfio.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gonhqaqtv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gvlygmemn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/goebbwzeh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gyprzcjsr.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gvgbgcboy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gfojwkdrc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gtbpfjhws.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gjltminsw.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gzohvvayp.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gertpecdg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gqeytnyfa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gfyuuyckt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gqcsxfnht.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gwhovnugo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gxfmimegl.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gyjvqqdkw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gxwgxvkji.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gfflshwmf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gfflgoymk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gavyhgjaw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gknkrxttm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/glpdjpabg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gfyakcykw.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gghubswhh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/ggbvtxbai.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/ggmdxvehm.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gvvhzkfzo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gcihmvkxg.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gibzqyqat.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gmbgbcuuf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/geliipfsn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gzncyexyd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/giasfjodw.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gzepmurqv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gfvyqjfbw.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gbjxbkwle.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gswdoltni.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gjdqhwcvw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/ghkbjcive.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gzrzihlrm.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gayuzvmog.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gkxsrulyu.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gtqhkjkui.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/ghgrncrle.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gpjoqfjqj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gtzlbrlvp.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gbksimysq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gvhdxwzjm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gxnrltfra.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gdhkuhmbg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gbdlmbtpf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gmhtqcylh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/glmzahslj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkbxnlqxd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gaveppcry.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvmgjknir.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/glmjkrdwe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gxmktvmbm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gfhtgbpzr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gomcgsant.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gzghzotex.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gfbzcwqvr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gxtmzcclm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gjszlbtpy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gdlsmviwh.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gksuxvikj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gsvycweac.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gbprqaxla.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gpfvypobq.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gmpqdprdn.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gpfhacjlv.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gphyrtibx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gyxhzguda.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/guvairfnq.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gxltzhoey.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gjanbkbew.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gftsxgrdu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gogronfmw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/glcrndnjs.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/goryepsrj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gqrlvspme.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gebsgdujz.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/ghqyvulzo.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gqxeyveex.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gownknubu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmfofsttz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/grcaonlxr.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gyrksacjt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gmikdcact.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gldvldeqq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/glqtwhyln.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/glnoeaqhu.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/ggiddeixr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gqrchahlb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gbnicwzht.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gluxbzsdb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/grsejtwkh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gsgppdjnz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gfiqiptuk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/giniiapgy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gbytwmwlc.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gsqekzwad.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/geifmruhz.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtbznfkqw.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gpkkolmuf.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gxfxyildr.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gfwmqoayz.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/grhpimjgf.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gwmtkixsb.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gisyzdirs.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gbcmoggmw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gwbtfnwgq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gfnzzulpr.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/glqswxfgb.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gcmzpqttq.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gxxbiorjo.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gyvkozdpd.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/ggtpgioec.sHtML


<!-- 参考信息 -->