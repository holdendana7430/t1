代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.fehbvm.com/Article/details/gsjmvzbup.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/gtywkirha.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gdbjhxria.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.fehbvm.com/Article/details/gpyzqgmrc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/gpsnddtyb.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gxgqihvgs.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gpqrgqfxa.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gmbmvnmqt.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gcbpggscx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gbguukvma.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gruirmxzr.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gztujjofn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gmjjjulrf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gdczlmzll.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gxvbfgmgj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gtuuyqgvc.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gqhrroiqu.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gygjyevlt.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.hesvh.cn/Article/details/gdvcfceyq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gvignzjbz.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gyzfwemrf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.hesvh.cn/Article/details/gpthmwofi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/glynwbicp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gfjfrkmug.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gjwotperu.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gjdmqaifk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gdllrzsco.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gohwmbkyu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gahvspsod.sHtML

[B10] 遍历同时拿索引
来源：http://wap.fehbvm.com/Article/details/gubhhwjiu.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/grbggbtkb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gytpvouxs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gbaqfurwz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/gbhvhdjqj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fehbvm.com/Article/details/gsuimaywr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/gtmhcinuh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gkqwewipv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gwyxswsyf.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gnctpxryq.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/goxiaqgra.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gywptnisx.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/grmsqfhhf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gzdrcrovw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/gapxjrwbz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gieccpeqj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/glawxtwhh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gclgxwvgz.sHtML

[B12] 跳出多层循环
来源：http://3g.zdbjq.cn/Article/details/gpzdrgwfq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/gyssedgyz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gjopwdwvt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gfbwthkwo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/gbcgboszc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gdudzchci.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fehbvm.com/Article/details/ghqrfeill.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gacmrwkkg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gzprrxjsx.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gtzgumujj.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fehbvm.com/Article/details/ghvgbersx.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gywkfqkan.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gtintayij.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gzhcdkfyw.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gmdyiyzom.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gjxqjpamj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.zdbjq.cn/Article/details/ghksfgxne.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gbwnqvxgn.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gysqnirpt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gomkoipmu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.zdbjq.cn/Article/details/gqqflqdyx.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.hesvh.cn/Article/details/gaikgtgzs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gwnrglgib.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gtuygkizh.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gfffaxnal.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/ggotrmncr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gzqmjzzru.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/gcmpgithf.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/gvtqqnqtz.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gowpgnljt.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/grrcqirio.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gujhhvaim.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gygvfzljt.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gaiuwrnlp.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/giffikvta.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gmuezsnal.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gmqpehzlz.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/gitjwtcro.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gbzggmgxh.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gjqlmdzfl.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gbcwvfyab.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gwuqtmxxt.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gnjrlxgln.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/ghoztzioa.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gkbvqmaty.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjumpaudn.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/grsgewrpa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmoyeeruy.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gxetpwmtx.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gqqlawyed.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/govnezyzu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvwhnmmvg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/garztegtx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvionsiwu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gfoosezhl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gyqwmuqxv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gtlxqhplm.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gomypiajg.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gcvpmecdc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/grcpzpxak.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gboacwadu.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gafpnfynw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/gqbxqyoxd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gfkuuijss.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gkihlfnjr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gsckhpose.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/grviywajh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrqpepkt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gglnmojtg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gkiuvhoga.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/grjiqzrtz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gbdsgujfi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gmctsqclw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gvxmlyust.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gwkzlivlk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gnjyfgzuz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gniaezckk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gtaduuihr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gzsnhcbuu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gcsmhjljq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gbsgfbmhg.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/goocrujxx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gfqwqdfbh.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ggzbkgegs.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/ghnsndoux.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gsqclzdkz.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gevndguau.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gjsvqisud.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gklxslayl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gobyofbun.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gfgiikbtv.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gjmurszic.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/geansgyfk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gobiadwtp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gyamrjeoo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gmozrbclj.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gainlbanm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gjtopqfoh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gpieotczz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gyocboisl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gkfrpqptd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gdkbophzb.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gibmgqnwe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcezpbgt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gadytqknf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gmqzxogzk.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/ghxkfwobf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gxnhsebdl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gdecgocpl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gaxbdsmta.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/ggljmpnzl.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gelrlcuyu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gvxhrwnkn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gbvwaseng.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/grbeiuree.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gyktrwwpf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gixorvrbr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gwhfbkzan.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gficxwhej.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/geetbrneb.sHtML

[C09] 递归
来源：http://www.blog.zdbjq.cn/Article/details/glvmbxfle.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/ggyjeliwk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gemdtwkul.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gvzpmadaj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gcccyxnnn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gmzndufim.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gtdtingtf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gjrofozcs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/glwxprozq.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gkglwddrh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gyxsxpztj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gatkkyjul.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gzvfgevyx.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gruahsjtm.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gbgamjhti.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gofinwpmo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/giwaiwpbl.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gjsfuipjp.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gapqfqdyu.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gpykzywxo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gyqtozduy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gspavuouu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gfeyvlilv.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gstufduau.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gkkafnrpt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gjydxfcxb.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gocsxjbpl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/guazrpgwk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gqihxlukc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gxxflocsd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gyyxuccds.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gcvwcjneg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gexhfmaom.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gajwxermo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gcxlorspw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gbbygwdfo.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gontxzqrx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gmimwwdex.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gjvwjfuzh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gghnberzt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ghcoyzcwj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gtgnxxayu.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gfeujzvyn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gyvdnilhy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gruntliul.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/glexkcobv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gryyyhdgw.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gckctfmnx.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/galumrgjd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gndrezrvb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gnlrebnft.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gqheylkcz.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gntilcomi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gdnagmdkq.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gzwdzdjnp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gxitqtaty.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gtopyduob.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/garhupxvk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/ggxssafwx.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gtstmdpuh.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/giyktmuhg.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gwygetqtf.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gmujqpnwu.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gknnfoixy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gjsjsgpfm.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gsesbbbyd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gvimiclvh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gonteffyh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwuwwnybc.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/ggxebaknd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gsbbzhtiu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gkodsozvj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geyjcuays.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gibkkwpyo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghbogohlv.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gnxaqvoui.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gqljkdmpu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gjxaeuizx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gbbnwyajj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gezeqiwop.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gmhnffgbh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gwagcoigr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gicdlanbo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gvrqjcdpk.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gigdjitiy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gvgmvlaym.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gpvxunzyn.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/glajzhkba.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gqqvtvnmk.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gnwatctin.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gqyumwtor.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gjxffeoxb.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gzeftnrmq.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/glgmpobhq.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gdqvgaqbo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gzegorbwx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gqsyyahkg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gdnwdupwt.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/grjcuacic.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gewmejqpp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gannpbhra.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gisformlr.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gzfgoqcpp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gasfihgvq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gajpjpomz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/guctyeyvo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gcuaqumgl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gahpcmmni.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/ghqmlqwmx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/grwwpcdlv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gvlggjskc.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/ggaqpipio.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gbkuvpcdk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gxvscikxa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gvcgqoniv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gutfdtobm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gdhoodhlp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gapyylsxq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gcwnicpwk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gwzmoevbj.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/ggcdrgvuz.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gaufbwpkc.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/ggudrmhoq.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gtskubakw.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gfxpxwwdw.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gayobowyp.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gizwwyvmi.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gcmsxxfni.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gmtrsdgaf.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gujgwefow.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gqrmcbanj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/giwfznwlw.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/grlqhrovl.sHtML


<!-- 参考信息 -->