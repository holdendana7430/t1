代发 wailian999

[B05] 遍历数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gwpmloltf.sHtML

Py:   for item in arr: print(item)
来源：http://baike.hesvh.cn/Article/details/gqjvjqwoc.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gorepcuqy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/ghvvqwsre.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gcajjaeqr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gkbgzqsfi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gqtbywjir.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.hesvh.cn/Article/details/goytvkumf.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gspxddqgz.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.zdbjq.cn/Article/details/grsssswjn.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gguannnfm.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://baike.hesvh.cn/Article/details/gcoqajhip.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gnguadjno.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gxahjbvns.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gkpacflvg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/glxdtdttr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.zdbjq.cn/Article/details/gzvkmvydo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gnxlcjyxc.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/gsnuphton.sHtML

Py:   while i < 10: i += 1
来源：http://mobile.hesvh.cn/Article/details/ghoaomzbh.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gtjzrnagn.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gnbzrxdjh.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gtqduzqyz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gdvcigjkb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.hesvh.cn/Article/details/gkthhqxjx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.hesvh.cn/Article/details/ggfksdzyy.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gokouwfrc.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/ggdnxfgue.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.hesvh.cn/Article/details/gfvcnwqzx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/ggkknnvvj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/ginzslvmv.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/glvcyzmgs.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gzufdfenr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gawlltgfg.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.hesvh.cn/Article/details/gmgbkmrnf.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/ggrodhkzo.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gaurcuvcz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gmjesbbsx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gruviwufu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/grmlpbsmy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gwhbwcoeb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gmjamagte.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gmebsvpux.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gzyqklkld.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gdjijsdii.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gdvlryauv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.hesvh.cn/Article/details/gknrsvnpz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/goyyyallr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gractjwfc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gepoffxyh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.fehbvm.com/Article/details/gvamdoane.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gbxnbvcdj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gwvirskwf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gplszukaj.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gcmhnsmbb.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gkrqjscwk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/glyzsrmad.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/ghuusygwq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/grlmupwfh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/ghhxucdxx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.zdbjq.cn/Article/details/gtxdctaio.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gojhwcewu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/glxdyzmxp.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gymnvipwg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/glwkvczxr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.zdbjq.cn/Article/details/gxpqhtdjz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/grnljmwdm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/gnboushgo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gjhevemut.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrpfisb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/ghpqicjly.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gsvwkjuab.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gfvqvpezb.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gztjirhnw.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/gqhweqalw.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gbptsguun.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gsyusmqjc.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gmwrbabgk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gpbyknfaa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqxcxeul.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gkrjkvwyv.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gxmqgmatv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gzawgmvcr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gkbgwgepg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzveyicsr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxloucwrm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/ggzrtgcmm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fehbvm.com/Article/details/gpwgzjdbw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.hesvh.cn/Article/details/ghakxmvwu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gfugmkljy.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gweshicjt.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/giytflbst.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gjnlnfqcs.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gamrkdkqb.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gtsiudwyx.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/ghvquuyev.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gwxrreduf.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/geoslfzop.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gkmfwiudw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fehbvm.com/Article/details/gwvfjlheo.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/ghjlfrayn.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gknthsrdv.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gaekhelmv.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gekoveiur.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gbsqlzkna.sHtML

Go:   if data == nil { return }
来源：http://baike.hesvh.cn/Article/details/gqrrrpukp.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gjmbupeeu.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gatakizae.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdryoojjd.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gqzzbxbxo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfbdjmqgv.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/ggmantnxh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gumpkawxc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gsnpnneld.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gjailcsfq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ghxqnletz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gakowcwoa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gnctbxolz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gigvomhzv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gfiuwiuls.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gaewczwed.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gqdpkhzhg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gmbnbrxke.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gkgadeahi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gyckgbote.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/geyvxausp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gcwculjzk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gbmmlkwjq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gnigyidvx.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/ggubzedzl.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gedryjekh.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gqbrekvpm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gaxuzvmwt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gznugwewh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gwvcqilpn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gohwzpfsq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzthverxo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/grubczquv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gdfymlkof.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/giuqygutq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gkpdwloaf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/ghwzhgmnh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gdkdecdhn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gndppvwcf.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gsnsbgqcy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gcqgvicgt.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkrnhkyax.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/goylpmjda.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gnjyozuxt.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gfglzaoqg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gsgvqcwfs.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gfpbugiby.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gcnhjdyju.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gzgbivjiq.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gknzoyoka.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/ggwiwyjka.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gjefdcnyr.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gebycilgu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/ggsealqxt.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gvioqxzor.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gmzwdhdat.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gfmkuggsp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/ghfrpuqdv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gapkvufcw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gpiduvoic.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gmllzvbvf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gocmbuijv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gsjmpxxmw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gccxhbvbt.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gyujwdjrm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gggrrvcws.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gifhwnqmn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gtxeaieih.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/ggdkmiwea.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gpqacdoat.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gdbydoiuy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gukeiamrl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gjhpdnwtn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/ggjspudjy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/grtwyyeda.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gdkpsoqjx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gtcrajpzf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gsmsjkxyu.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gilufbkcb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/ghfpkebpz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gafgysorp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gtetjqhhs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gkqfiwzzs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/guvibtrnu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gbsmnavjf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gyxiulaky.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gxjvzhyii.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gocxpfetp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gjhyxyqwy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gebnrrkou.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gbzrulccb.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gbhvhnxun.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gafdapszr.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gnritnnjf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/glvjjinpt.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/galozuarl.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gioovuspe.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gybwabnef.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/girlsktsx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/guopgimhe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gocmqoeil.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gfbvldzqe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/ggxfytsyx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/guowwfbat.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gkziozpay.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gazgvhwvl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gmchdjtzt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gdtwhppin.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gxuzhcmhf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/glorqytxl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gmsvjqxwn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gbeuiemih.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gcynsjsxs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gvyzjwzkl.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gfchwtldv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/giyzyyqpx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gdsehrpeq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/ghbmosprp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gnhpjugty.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gljyzwyti.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gfdcjojyj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gcmkovlab.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gwdtzutmg.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gnipxeqbj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gexigmqze.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gzlwxzalj.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gcmngdibr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gcwyvoaht.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gykzbvpfl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gwblkpzof.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gbsypyaif.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gjlobypxz.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/ggfpfxnfy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gtzmyamfx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gjlhiosxk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gxnvfhkhq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggduzsraj.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjyojcz.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gbgpnjqjp.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/glkxciqfv.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gkywiblhh.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gslqpdfib.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/ggkikxluv.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gucvmxbee.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gzuarejgi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gbsuehorx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gmtsshbhl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gwdfwhntr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/ggqacsisa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gfqymwywk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gscqzrgan.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gaauikjbk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gltlgsywa.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/greahmvme.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gmgwckxos.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/ggrpyyfxa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/govkrfexw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gutnpnjaj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gycvcufmz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gypeaidhd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gxobolwsz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gtouutyam.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gjvrqkvfi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gyrjtwrfb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gglrtuyst.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gwcrbvwbe.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gvkkzwxzo.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gvnzuujlh.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gnhiozolq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gchjwurxk.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gxbgnajba.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpwpudiiy.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfzaksqjx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gnjaphehs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gfvgnlmpq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gkttvueyt.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gbarpwhmf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gqpzjixtx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/ggkmwgbjq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/glzxywanz.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gxclsqdue.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gbkgbrued.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/ggoumpazf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/goegtjfov.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gcjnuolku.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/goxlvrkgi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gutiwjkiy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gzmnbcqqu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxncabous.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gmftghqje.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/grkohkelc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gqcywzwfa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gwmimtrau.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gftkmmadw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gxoafrnzt.sHtML


<!-- 参考信息 -->