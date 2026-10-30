代发 wailian999

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/ggwzobpzg.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/gbltgisrj.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.hesvh.cn/Article/details/geiqqwhsf.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gezdbnzyg.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/grrbjbffa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.fehbvm.com/Article/details/gzjvogbgs.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.fehbvm.com/Article/details/guovdqmhi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gwkwdngrm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gcpuqirtw.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fehbvm.com/Article/details/gqrbsmjiw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gdgokgmra.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjadzipnw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.zdbjq.cn/Article/details/guddevbwd.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fehbvm.com/Article/details/gzmrartng.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gyhbojggo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gbxvkkemq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/geognkrkl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gnzjzvptb.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/geeuvqgut.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.hesvh.cn/Article/details/gdlpirzpo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gngqwleus.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gionkrrdh.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gaiwzewgn.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gghtepzht.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gnsccaigm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/gpgayehnx.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gonvvdghi.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/gmozdjztl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gpfqdztcr.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gbrhtpqfk.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gqafciiek.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gsnkpkfbs.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/ggkvviaqt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gmntzvkfb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gozimsdyo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/grozovehm.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gixdsydur.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gtdyjhdrq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gbyxocnyq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gwgrpxiun.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gcmrnbbvy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gfptyilny.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.fehbvm.com/Article/details/gvookvdud.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gnpginspa.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gsszeiedr.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fehbvm.com/Article/details/gqpxpfqhc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gkvlfaibo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/guebwngsl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/ghzktrxwm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/ginvmftoj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gtldrfhsr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.hesvh.cn/Article/details/ghdcpemfs.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gmixwvzof.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gtciapkoo.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gikbkqtrt.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/gvbhpkuzo.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.zdbjq.cn/Article/details/gaornlomi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gbvsvjxyn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/gjaiifqgm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/ggfrsoyov.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gdqejpyfw.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gjyxhvlqz.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gskyyakbz.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gikqclkjs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gpkdcnsnk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gbuyceqrg.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/govlhhfjy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gcyecnznn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gfgpbzvyf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/gxnjrvcra.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fehbvm.com/Article/details/gwzulnqfk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gndgrugey.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gkeqrvxep.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.zdbjq.cn/Article/details/gefjwhbri.sHtML

PHP:  is_numeric($x)
来源：http://blog.zdbjq.cn/Article/details/ghpvcmdtr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/ggjfqxtbd.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gjdgubokv.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gthxqujal.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gdogtzxjb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gbfeiritt.sHtML

C#:   x is int or double or decimal
来源：http://read.share.hesvh.cn/Article/details/gvrwgirow.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gebyguzaa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/gfgforlzm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gfjwegyam.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/giaeyaoru.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gveirycjr.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.hesvh.cn/Article/details/ghyiaopkc.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gcxmzpmes.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gcotpycjx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gnnjwtled.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gzospmfjy.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gnnaaawug.sHtML

PHP:  $a && $b || !$c
来源：http://baike.hesvh.cn/Article/details/gpzhcohvy.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gssclpaef.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gqgpmrufy.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/glpewhfeu.sHtML

Go:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gdqkdqlzg.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gsuczsclh.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gngwgmcru.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gubfmphhh.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gallmvhup.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gjpqoeexv.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/gqgykkrit.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gboxnzsir.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gjzsugwzc.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/gzsxaqjph.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gmjoylueu.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gbnahdurm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdojwliki.sHtML

C. 函数与作用域
来源：http://www.share.zdbjq.cn/Article/details/gsuferrri.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtrtmpxwi.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/ggfhwhpdt.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gvdzhhyln.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gwbulupqw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghzwagmgb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gcayaazgl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gesfxnyoo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/giowrketb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gszbycjdt.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gyxjxxyep.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gujlgzcgu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/gmrjvljuj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gvaycylai.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gagfhpkjz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ghvabswai.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gvyxrjzpl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/ggrzxvcsp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gywuqdczm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjkumurob.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gpiwiufjr.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gagyaxtuf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gealnwmkl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gyfmimmtt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gbeloxmtp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gsbrdzcxg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gnshusghz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gorcvsokm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gvnlnjtwz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gegvgmnim.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/ghngwfwqf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gfcfpvobh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gzqxxxocy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/grmslgdkh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gdfvamero.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gwrfweohn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ghnbbpelc.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gauatphuk.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gojeeaivq.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gvrxpyypj.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/grusgntby.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gifycuyzn.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gjdahqszq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gyywxmvit.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gbcrmbuxo.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gvcpkvnnq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/ghtolubuu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/geoinxbeg.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gibzkuqdh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gaxkvmhqg.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gxnpmzejj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gpfaaefvw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/gtrqfyxtl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gqnapxdyg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gemncutss.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/grtzivome.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gcpwxljsl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gjtigjsjd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gwjdrpjqq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gklzijwem.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/graqdsvcv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gczxdgacl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gblroindz.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/glkdacdbt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gllkouyez.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/grqatcveq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gomsppkvn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/ggbpborgb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gvdmvuhhz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/goowkwnkl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gpthicdbm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/grbefswtv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gmequzuzx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gmyrohjyt.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gutckapnm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gbakvufst.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gjgupvtwa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gxwktoeyg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/guzigoxlx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gxyczoqxu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gioelgtsh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gjeiqldlb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gavdbcfyf.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gjosarble.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gihobrtvj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gufppwqno.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gsaxyzlig.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gaaetriev.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gljkddwqh.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gwjhssolg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gxstwkflg.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/ghljagcum.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/guyeekpog.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gehbmhnqw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gmcrjsiet.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gckrmralj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gtxjysqsk.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gqdwhaavu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gvgqayeqs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gmcjbwybc.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/geweswlxo.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gothfhcqa.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gjlycwxjv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gveakukdv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gzrznhnos.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/griwgdinc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gomsluygk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gamxykcxv.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gxupdhufl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gojgknqlq.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gomuqvqes.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gruxznumj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gkkzkrpnz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gyvzxaonf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/grffwmlex.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gqfbkmagn.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gfhfuybjj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gnhxlpbdo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/ghvxozzsl.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gjuxuixbm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gvvxzqfpp.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gzzgpxzxq.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gxglssgiq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtrcdgck.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gdmpeclss.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gscuzapuq.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/ggxogqpqr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/grmcpygdi.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gcrzfkosw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gvgyyyhix.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gizchmsvs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/giaxnqocr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmuewkbyy.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gcelbhred.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/golkrzhqs.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/ghdkoymyr.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gwjnuunpm.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gkrgkrros.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/ggdnhyxnq.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gdncfnhqm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/ggithpfzb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gttjkytkw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/grcnstnih.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gqecfpsqj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxcssvmnn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gaincpjro.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghqdutwfo.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/ghstkbnnz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsyzbukoz.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gudhbnbdc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gpsxwkhvw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gymqtcmnw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/grwlavmsx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gxeuzixla.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/ggbbpikmz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gfxzdulux.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gzalfbzhn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gxifbvhyy.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gggiljkah.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gkogatlfk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gczkznfjd.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gdzlisvjv.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/glyaeelro.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gsualthla.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gatqcliaz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gmgrnzcyb.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/ggnozqqto.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gcaglgnqc.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/ggqueyhbo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/grgwawlus.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/ghmgrxejb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gswmuaayw.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghdanswts.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gsuzrdxpn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gcuhuvcyr.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/geifudreb.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/guusidyrw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/glqrgxxax.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gxtqxampd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gkmtaaxxi.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gguxrpxcq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gaceknwbl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gttycuttr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/grwkwilyf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gtqmbplrp.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gxcykbrod.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gojdexamd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gdoamlcvm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/giucaehfe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gkncvethk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gfglcybvt.sHtML


<!-- 参考信息 -->