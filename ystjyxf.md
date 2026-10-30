代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbrvujrr.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkfxtpjo.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwyikcxq.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.fanxiaobao.xyz/Article/details/gskowekvz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakzxiljo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhkuocgw.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyhxnwtv.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fanxiaobao.xyz/Article/details/giayfhsgt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fanxiaobao.xyz/Article/details/gtcgacqkn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gpfkrspnt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlxthjcn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gfshudmyr.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/giujmkyxi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzcghrod.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gywgeabup.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gypwvptcr.sHtML

[B09] break 与 continue
来源：http://wap.fanxiaobao.xyz/Article/details/gljugupic.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gzjlmguuz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtttvychw.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gztkawucm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtsizmyvr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtcluvlk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fanxiaobao.xyz/Article/details/gejhaqwix.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fanxiaobao.xyz/Article/details/gqonrdurv.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqmketmsy.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvrepsbz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fanxiaobao.xyz/Article/details/gpjxjqssr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fanxiaobao.xyz/Article/details/golbgugor.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkswzxyq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/guailoeuz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gytretcgw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fanxiaobao.xyz/Article/details/grlxpehel.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefixxolk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqcrflxh.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fanxiaobao.xyz/Article/details/gmtnodraa.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskxxggzs.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gmodapzrc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ggrifuvjv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiplkkcf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/ghbadpfwt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fanxiaobao.xyz/Article/details/gilejehnv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/geevxhdps.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gwsumsegy.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/glzckqajo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fanxiaobao.xyz/Article/details/gegspihis.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmakxodrc.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gfwaodpxy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gosvzppuh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gednmakrd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gymuxkwve.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gmutpmfbf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fanxiaobao.xyz/Article/details/gueeufaqo.sHtML

[B13] 判断是否为数字
来源：http://blog.fanxiaobao.xyz/Article/details/grizxkauk.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdvazygh.sHtML

PHP:  is_numeric($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gijkqaskg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhieqcuz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gazecbrnj.sHtML

Java: x instanceof Number
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhecvaar.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/grktnbgeq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtecplqfn.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grssrzttf.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmdypymw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcddodtu.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fanxiaobao.xyz/Article/details/gfercxety.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxsxazla.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasoujtgr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpyjbhay.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gndxdxmjx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gokurcfzq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gstpthtqo.sHtML

[B15] 布尔运算与取反
来源：http://baike.fanxiaobao.xyz/Article/details/ghriipifq.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqwjxvfj.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlrihpnq.sHtML

JS:   a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gniqoahnd.sHtML

TS:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevtqqepu.sHtML

Java: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/grhjwqnxt.sHtML

Go:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwsxtsam.sHtML

Ruby: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmeovuwt.sHtML

C#:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gjdrjbvdp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gszzggszm.sHtML

Py:   if not data: return
来源：http://wap.fanxiaobao.xyz/Article/details/gbapgstad.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grpxgdcvd.sHtML

JS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/glwttgpug.sHtML

TS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gzfrldumb.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/ghapypfvo.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gurelonrb.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshfneonq.sHtML

C#:   if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gewxsuvjo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcpxgbojb.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxossxjw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuroblay.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwdwpxllm.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/grvotsobt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxkqyhsd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/getgvcfiq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpqxzhdt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gktutyztd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuyiglvm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffeztrpj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpgjczupc.sHtML

[C02] 默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzkgclif.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fanxiaobao.xyz/Article/details/gslgdwrrz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giepuezah.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/guezgspyn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwmvkghwz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjxxfkfy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gcotfrqma.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxxtffaw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlecfizi.sHtML

[C03] 可变参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhyreaco.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fanxiaobao.xyz/Article/details/gjekywfxy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxxtlnxco.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gruqteylj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gcrdcknez.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqficssy.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fanxiaobao.xyz/Article/details/gmcdcpubl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsudegoyh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fanxiaobao.xyz/Article/details/gswpijghg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gapnnjohn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fanxiaobao.xyz/Article/details/gkivrlshh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/ghcbwhdey.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvsvyhaqh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnojgoyx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fanxiaobao.xyz/Article/details/grrjtigdp.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcepdplnf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdsxcwlty.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjxfznpln.sHtML

[C05] 返回多个值
来源：http://wap.fanxiaobao.xyz/Article/details/gcrpfbxtn.sHtML

Py:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gukbrmboz.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/gkwdyxcrh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvkkryxw.sHtML

TS:   return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gxulfambt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fanxiaobao.xyz/Article/details/gcencblid.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdiyuxnn.sHtML

Ruby: return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuzsxjhu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/gkclflepo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdbmvfrl.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxgxecff.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjodjzbyo.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gkiispczu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gichmpofk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gwbvbubqt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/ggeqesuil.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupzdkzmr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gajadysih.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gucjiqizn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fanxiaobao.xyz/Article/details/gyukirahj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqclphitr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjuexpmr.sHtML

TS:   arr.map(String)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgcqchug.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gjcceqopc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/gxppemobz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqfyzupi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/gevnexpra.sHtML

[C08] 闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhkjxgkh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsxlflmn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghoxwsvkc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjujpitqc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkygkquh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/gnliumpqz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fanxiaobao.xyz/Article/details/gwzbcogqp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fanxiaobao.xyz/Article/details/gflnjhztw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvsjisgg.sHtML

[C09] 递归
来源：http://3g.fanxiaobao.xyz/Article/details/gxifvmnlf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfukoamj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyapnicmw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmbxjmbs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gkhpltcij.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahztglym.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtysxxnzh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgyxhnbf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgjuzurb.sHtML

[C10] 变量作用域
来源：http://baike.fanxiaobao.xyz/Article/details/ginxhiydb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fanxiaobao.xyz/Article/details/gptxuozwi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fanxiaobao.xyz/Article/details/gzajvczwj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfjjebiy.sHtML

TS:   同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gxloiafeu.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gzscuqxpv.sHtML

Go:   花括号块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gqsgkkewv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fanxiaobao.xyz/Article/details/glqfvunuo.sHtML

C#:   块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gvjakotqa.sHtML

[C11] 模块导入与导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiziituv.sHtML

Py:   from module import func
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsttucpxd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcokrgqxv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gohjknxyc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fanxiaobao.xyz/Article/details/gjwddzgrm.sHtML

Java: import java.util.List;
来源：http://baike.fanxiaobao.xyz/Article/details/gxcwjziqm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fanxiaobao.xyz/Article/details/gjamjmmec.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fanxiaobao.xyz/Article/details/ggzcprtqu.sHtML

C#:   using System.Text;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxebwrgc.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fanxiaobao.xyz/Article/details/grnievhhg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guenmrcgk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fanxiaobao.xyz/Article/details/gaadtptty.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkeyqaoy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/guvevceyg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fanxiaobao.xyz/Article/details/gjumghsuu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fanxiaobao.xyz/Article/details/ggziiqdcf.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fanxiaobao.xyz/Article/details/gntppxkas.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gctytdomd.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzptxbls.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gfqpakyef.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gykdakbso.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmulyavk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjjxtkkvh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdmmidanz.sHtML

Go:   func add(a, b int) int
来源：http://wap.fanxiaobao.xyz/Article/details/gfrnymcvz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzltcagt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybcemvmt.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbsfhlhco.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fanxiaobao.xyz/Article/details/gxprbfwge.sHtML

PHP:  // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/ggvlujkih.sHtML

JS:   // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/glxrqsfhs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gypohuzrn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbttiuofn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gksursnwn.sHtML

Ruby: # 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnzngxsv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fanxiaobao.xyz/Article/details/gtkabcgej.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fanxiaobao.xyz/Article/details/giiqgfqnd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fanxiaobao.xyz/Article/details/geqpxakwg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsmgktmh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnepqbtfs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gszhadtnq.sHtML

Java: // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gsexidkcy.sHtML

Go:   // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gwguuydme.sHtML

Ruby: a, b = pair
来源：http://read.share.fanxiaobao.xyz/Article/details/gesvsnpes.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzilpvoyy.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fanxiaobao.xyz/Article/details/gjhvbhntv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoocjdie.sHtML

PHP:  // 无重载
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdbzhaaa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gaetkkyhb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/gjqxuslwi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gygtcswpx.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmhjxluh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgmcjjjt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnasrvqnf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxpikajj.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmvgsvzt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gscwhgoaz.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxqbkspm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fanxiaobao.xyz/Article/details/glthzguds.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaajgmfb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gbloanyqv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gkxdaoyay.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/gsneghmmf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfegrkvxt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gincjhisb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuiubehx.sHtML

[D02] 追加元素到末尾
来源：http://3g.fanxiaobao.xyz/Article/details/gsbnkpmao.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fanxiaobao.xyz/Article/details/gtsiahdgn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnythsxic.sHtML

JS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gcihionvd.sHtML

TS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpkmbsjq.sHtML

Java: list.add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gxkwrdcup.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/giacsfvkr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgwbphle.sHtML

C#:   list.Add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gotmrsqrk.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfvwbbzu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gkdsagnud.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gzgobargz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fanxiaobao.xyz/Article/details/gqspdpjca.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbxgnkrj.sHtML

Java: list.add(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gbwpwignu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gwbcjscxc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/gmrctzvim.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/ghgpxrywi.sHtML

[D04] 删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmhvhfyl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxqvfzcw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgxoiulo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvrutojc.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gnipxeoux.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrzyvgmh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiflgpbw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gfldnthei.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbwzbphl.sHtML

[D05] 访问与修改元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrlnrsss.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhxkkaqe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gfizefjfp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggapkdsoy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcstxtxy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glktzmsqv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gevupjfgt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgmoxqrf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/geuhlsvlg.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gqcsgjhol.sHtML

Py:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfhgmhpl.sHtML

PHP:  count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gktfohuxh.sHtML

JS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsrvpvpn.sHtML

TS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/grewsfsry.sHtML

Java: list.size();
来源：http://wap.fanxiaobao.xyz/Article/details/gmlvepmmw.sHtML

Go:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gyctbkupi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gnepvtzih.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/goxarkxzl.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxpfvdbt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fanxiaobao.xyz/Article/details/gtsxzbxpm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwsdurbg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfcaabih.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gyuzvzlnz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwpgcrck.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/gylzgsosx.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/guqltplfd.sHtML


<!-- 参考信息 -->