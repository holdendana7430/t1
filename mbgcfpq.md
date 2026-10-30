代发 wailian999

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gepvnubgu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgqbmfiz.sHtML

[B07] while 循环
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkmaglod.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gokfoayho.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glegberhj.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/galdjoham.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gattzdvpi.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsvjkwsm.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fanxiaobao.xyz/Article/details/gayyriyyy.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gydffjzuc.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqlknuls.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fanxiaobao.xyz/Article/details/gwjfizjnb.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fanxiaobao.xyz/Article/details/gogngmjls.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gmevsbxqa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/gzsqprcuc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.fanxiaobao.xyz/Article/details/gscwqxlyx.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/grxfmxoha.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gokqqjdhq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gbimiwssw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/goczzkkon.sHtML

[B09] break 与 continue
来源：http://blog.fanxiaobao.xyz/Article/details/gmgnvxnxj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gkxitmtpp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzotrpvlr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxybbbzw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gshrvpcce.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fanxiaobao.xyz/Article/details/gopziavqr.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkrnktbr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxmoxiqj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goegnwuyz.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhusdyhn.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.fanxiaobao.xyz/Article/details/gedrbowku.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbpzrmra.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gtslnhear.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fanxiaobao.xyz/Article/details/gmaatdsvq.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.fanxiaobao.xyz/Article/details/gkpwiobwn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gxdawyysj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gseodxmyb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwbciaqdv.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/gfayxywkq.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.fanxiaobao.xyz/Article/details/gwdevaeoo.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtgmvmpm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gpkcudfbf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfxerope.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipzjtiyd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecmxnyyp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggilxobkm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gluvcfora.sHtML

[B12] 跳出多层循环
来源：http://blog.fanxiaobao.xyz/Article/details/gnnqbqxsu.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gzfoahpze.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gvjqjszoe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkqqiyuj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupwoyqdo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/grepqsump.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goijrkntj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fanxiaobao.xyz/Article/details/gcxvqcyvn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gnzkrbwou.sHtML

[B13] 判断是否为数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgpkdiuh.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fanxiaobao.xyz/Article/details/gbhhpcrrh.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsoswsrg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fanxiaobao.xyz/Article/details/geazxtcmd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/godfpprif.sHtML

Java: x instanceof Number
来源：http://m.share.fanxiaobao.xyz/Article/details/gdntwqcvq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/givjanjbl.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfjdczum.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fanxiaobao.xyz/Article/details/glbzzboye.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/grsrmbxih.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fanxiaobao.xyz/Article/details/gbekofysi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlxelavl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/glfabfmgs.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gicjembjn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbhzdxrw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gdlzxrliz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbzfhhio.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgnelrfy.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlrhrpum.sHtML

Py:   a and b or not c
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyrzcvhw.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyretcfx.sHtML

JS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwjubtfd.sHtML

TS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gilpwesvo.sHtML

Java: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxkhxspl.sHtML

Go:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glblwwsky.sHtML

Ruby: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gsmtnecxl.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gjesldnkh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/gcyjxhxmi.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimvqstsp.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxizcvlht.sHtML

JS:   if (!data) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyxgmxkp.sHtML

TS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/ghwisyubb.sHtML

Java: if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gueskyodd.sHtML

Go:   if data == nil { return }
来源：http://3g.fanxiaobao.xyz/Article/details/gebzhbidf.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/garbqkxgn.sHtML

C#:   if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbctjblu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmowmjdm.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gdlyvncdk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gaakuqejp.sHtML

[C01] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gruhskqrd.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfbdckuh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvyyiegzq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwiztmdz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmuvthzjo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gszvdaebp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskfrhgoe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fanxiaobao.xyz/Article/details/ghnnbyutl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gufdekohe.sHtML

[C02] 默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gafcncgdz.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/gmmjjyfuo.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gweooockm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvgsvazp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbtqtefk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gagavkaec.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmtshsjnp.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fanxiaobao.xyz/Article/details/gsqctzgxl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fanxiaobao.xyz/Article/details/golfoyfrb.sHtML

[C03] 可变参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqitsuwa.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxjkuner.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtiluytcv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/guhextdyi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gihvjgjdn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzlcqtwm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjqbbbpf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gipalukmu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyutnpxv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkwjcsma.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvuzrhah.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmmnkduy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/grnnorrmu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjcwrdmv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fanxiaobao.xyz/Article/details/goewwjebv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glmcjziqw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjvcexiu.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzywpzyr.sHtML

[C05] 返回多个值
来源：http://www.share.fanxiaobao.xyz/Article/details/gmigdeurq.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpecwcphl.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxqpqfdo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtwzlriw.sHtML

TS:   return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gxxiahjez.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gswgtbhpu.sHtML

Go:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqdgguee.sHtML

Ruby: return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gezaevmcv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/glsvvnmnt.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/geimosluh.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fanxiaobao.xyz/Article/details/gvmoqxyim.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gxixblwfa.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gimaaiirb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gtrwththe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/girnuclez.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpvccwtu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gesetydmj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkuwfknw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fanxiaobao.xyz/Article/details/gixfeqixi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fanxiaobao.xyz/Article/details/gvisjqtpt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfowtmams.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fanxiaobao.xyz/Article/details/gmmccgyna.sHtML

TS:   arr.map(String)
来源：http://3g.fanxiaobao.xyz/Article/details/glegfavql.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gneswmgdx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fanxiaobao.xyz/Article/details/ggbzpqlsl.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlrxripq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fanxiaobao.xyz/Article/details/gmvqvdnhc.sHtML

[C08] 闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gadchehre.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fanxiaobao.xyz/Article/details/gxosdadxi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntmwkcic.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goaaleeeq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmszyjjxd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fanxiaobao.xyz/Article/details/gwwyrutbs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbtegmwz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcswuwpa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giuklminf.sHtML

[C09] 递归
来源：http://baike.fanxiaobao.xyz/Article/details/gzptpkrhe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggvwrmrak.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/ggitkbvbu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfffkqxw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gdvardbst.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntkmjdji.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fanxiaobao.xyz/Article/details/givpserjl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glffhsxlp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gupwkbdnf.sHtML

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gihybgtwh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/gggjvkytv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fanxiaobao.xyz/Article/details/gsncomrue.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/goybdduik.sHtML

TS:   同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/gefkxnpol.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbyobcot.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/geuxhyedf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gkedeoppo.sHtML

C#:   块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtnbwdjz.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxrwubqy.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqfkwpqk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwhpsjmw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gedemahkb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fanxiaobao.xyz/Article/details/gonkmymfq.sHtML

Java: import java.util.List;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqxwdrej.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjkblavv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyidrihxi.sHtML

C#:   using System.Text;
来源：http://wap.fanxiaobao.xyz/Article/details/gyhxurnnz.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsxhcqdd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyfuykqy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gixpsslvl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhdswlgo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/gvdawsqfa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fanxiaobao.xyz/Article/details/gotebwqaj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fanxiaobao.xyz/Article/details/gazlhazsh.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fanxiaobao.xyz/Article/details/gbvscldyr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqfbppjoo.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fanxiaobao.xyz/Article/details/gwkxyvmtf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gpiyxywtn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpcehfadu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fanxiaobao.xyz/Article/details/gwfhljvtd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdipnobjf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/grwwbhutl.sHtML

Go:   func add(a, b int) int
来源：http://blog.fanxiaobao.xyz/Article/details/gzugonjjm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvveuntx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfinmqdsw.sHtML

[C14] 泛型函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzjksdvh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjrsbdkx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfjbfulz.sHtML

JS:   // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gyzutfdek.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhlbzlfd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gftleouri.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fanxiaobao.xyz/Article/details/gdgzniwga.sHtML

Ruby: # 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gflwuoqzp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fanxiaobao.xyz/Article/details/grijhngth.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpmnevqd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/grwemhpej.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fanxiaobao.xyz/Article/details/ghunkdvmg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gohxwcjzv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gefofhghc.sHtML

Java: // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gzrvotmqe.sHtML

Go:   // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/glfjhpevt.sHtML

Ruby: a, b = pair
来源：http://read.share.fanxiaobao.xyz/Article/details/gemmkkspf.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/gietwesyl.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvefwzdz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fanxiaobao.xyz/Article/details/gaitlhjbo.sHtML

PHP:  // 无重载
来源：http://wap.fanxiaobao.xyz/Article/details/grovjvqiv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gjdobiyip.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvpemiye.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmriyita.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpopvnccw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fanxiaobao.xyz/Article/details/guyocroui.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqyogahob.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guiyldivp.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fanxiaobao.xyz/Article/details/gvdqaoird.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswddzhpx.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gtwjzinvz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fanxiaobao.xyz/Article/details/ghpfzctxj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/glqchkzxo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gfnwgohth.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fanxiaobao.xyz/Article/details/ggobkpuax.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fanxiaobao.xyz/Article/details/gezarrcpb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/ghealfqch.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gldveidks.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/gngbsawfc.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gssdpxrye.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fanxiaobao.xyz/Article/details/ghgsybodi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkztqxcl.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfxdxenc.sHtML

TS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtncwhtki.sHtML

Java: list.add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvijgenfc.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gchaierio.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fanxiaobao.xyz/Article/details/gqmrsyyba.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/ghlxdziyo.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fanxiaobao.xyz/Article/details/gbaqmtnvg.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/glqnkwzvc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/giyjpivko.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fanxiaobao.xyz/Article/details/gsravbhlo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkktkihld.sHtML

Java: list.add(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggielorqe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gkdabeacm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fanxiaobao.xyz/Article/details/gfnjykhcu.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gnupcvbrp.sHtML

[D04] 删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gdtuwigbb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrmqdqsn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gajkdzfbl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fanxiaobao.xyz/Article/details/gtoqvfyjm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyonyfob.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gquqccast.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnywhvguy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gkmoqtddr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fanxiaobao.xyz/Article/details/ggdtjpoai.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/gmkkjqpqf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gzjqscspu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gouhrstxe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxzidcew.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fanxiaobao.xyz/Article/details/ggrkkchiz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fanxiaobao.xyz/Article/details/gwymxnqzb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gakspaiuk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gmflisssw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gnuuhztqd.sHtML

[D06] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gznlmmfnu.sHtML

Py:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/guiyfuqpq.sHtML

PHP:  count($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkzcanmn.sHtML

JS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gmusvrivf.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gartyeayi.sHtML

Java: list.size();
来源：http://blog.fanxiaobao.xyz/Article/details/gqekgwyub.sHtML

Go:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnehaggo.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gcbukpfms.sHtML

C#:   list.Count;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzjnikhe.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzicfdtm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjeneejg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgdlzxyf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhrfskpz.sHtML


<!-- 参考信息 -->