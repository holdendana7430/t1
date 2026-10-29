代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gxsouaoxf.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fehbvm.com/Article/details/gpmygykej.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://3g.hesvh.cn/Article/details/gvnyknuwp.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/godvcyiha.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gqidddkwn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.zdbjq.cn/Article/details/gszblgyll.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gnozujhci.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fehbvm.com/Article/details/gvhtrkttv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/ghkizkqug.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.fehbvm.com/Article/details/grysxksdc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/gtvexumpw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gdyhtooga.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gjcjfdpab.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gsbslcwry.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/glgofwbrh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/gcjfobzgn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gzixmycjs.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.fehbvm.com/Article/details/gipzytqwa.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/ghjbwzpxm.sHtML

Py:   while i < 10: i += 1
来源：http://blog.hesvh.cn/Article/details/gzrloiiff.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gnuyzpirb.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gxyuhafng.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gfwqoqczt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gxcxxzzye.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.zdbjq.cn/Article/details/gtqkugosn.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gqcfxvnhd.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gbhjbcmcq.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.zdbjq.cn/Article/details/glwvwslao.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.zdbjq.cn/Article/details/gflggntki.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gwfllqvge.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gdratctpu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gafzrjdav.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gduvgvpjj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/grahfyhux.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.zdbjq.cn/Article/details/gpemrnwrz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gajpervue.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gmbshyxzv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gffuwkzed.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gkibfbrbq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gvggqcgmp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gowgapqtz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gzaztdfcm.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gekvjdwwl.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gdqbnqbas.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gxavpfsrs.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gwxueuwva.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.fehbvm.com/Article/details/gwnisdsqm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gcinhjfgh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gecngjshy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gahgsdrwj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.hesvh.cn/Article/details/gzdcvbshi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gpmftmogm.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.fehbvm.com/Article/details/gptkfikji.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gvraqcfpx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/grdkgffpe.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gynjxbdpe.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gafwvyhtz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/glhjrumra.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gegnsayrh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.hesvh.cn/Article/details/gxizgvbqu.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/ghlegvnin.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gmqwficdw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gornlviuf.sHtML

[B12] 跳出多层循环
来源：http://baike.fehbvm.com/Article/details/gkggvzijv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/gyhvkbsvr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gmzikusdx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gmjrcgkmw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gkkxvevfa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gjcvxjziv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gtulfvlhz.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/gdktjzrpb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.zdbjq.cn/Article/details/gpmxrvycw.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/giwqzlhol.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/ghknkgtqg.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gzqfsryrq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gsmojjund.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gwosgokdh.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gussrdvwz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gfiezfcxn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gmscsetww.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gufztahha.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gvcrixelm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gfdydxjio.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gyasjxpir.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gpogvpxqo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gxvsqhsdd.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gmizciowj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gasevkirk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gwophaxpq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gqsvckqta.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gltkbnhhg.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/giaustgob.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gxjyymtnv.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/getlilvjq.sHtML

TS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/guynqjzwq.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gkivegqes.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gurimgmid.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gvrrbaakz.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/greirxgpf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gltvxxlyp.sHtML

Py:   if not data: return
来源：http://www.m.share.hesvh.cn/Article/details/gwpgqmgqz.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.zdbjq.cn/Article/details/gziakbbma.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/girpcpisc.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/ggpiwbweb.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/giqhasxtp.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcmgrbsb.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gimvztllo.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gqpqfbxvn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcxhuxamx.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gkndljgdm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giygsfgxj.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gloxlspxl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gwtxiizwv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gveerdhsd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/grxwoumip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gxiovxrkd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/glgpxqigb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gytbkxyfl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gkxtczvof.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gmstdfpdc.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gkdfhhxcw.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gujxrjhmq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gsrovhxcf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gbqjnhbft.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqhafbwlp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fehbvm.com/Article/details/ggpujczvu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/ghudxvmba.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gsvznmzim.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gkletuqnz.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/grsklcoaj.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gykthokql.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/geavsuwrx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gbjzepgbf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gcdzxlmmz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gbqilkjae.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/glslxelxi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gryhyusll.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/geshyimxd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gdzzrnegn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gpzqxyjml.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gsaztuhbb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gqhuloinf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/gblturush.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gfarhtzxm.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gejymyfjk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gfcbhfstd.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gzgxzeabs.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gsoojitgx.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gtcxxqtge.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gkbmxjoic.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gacxosztj.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gcwqstuuy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gvubqpixa.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gjqwoekmn.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/grpremytv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gxvwjgogm.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gagrqdsta.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gfsifensl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gtjyrqkzu.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gqlkgdrxo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/ghhibjuto.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gygzqemjz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gtgbapuxg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gocaphwwk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gytogxdxc.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gtcmgbtym.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/ghxwbgiiv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gyfsxdvba.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gbaujfvgj.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gaxzgmwui.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gajdirzwz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gkniohath.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gzkjwdbcv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gnsalqulj.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/guiadkxvh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/ggkgxxsbg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/glrlmpjtp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gxkymwtet.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gdciesefz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gxzodgxrq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gldswnquo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gmsvfmaix.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/goktxpyhb.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gcqfugwlu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gnofquznk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gydapsyht.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/ggzrwpdlr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gagbuwzdy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fehbvm.com/Article/details/guhvbpoxh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/ghtaksbgs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/geasrcuhb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gxrqvqtrr.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gkjniaenf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gfluserlw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gpypfypjx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gzkuznxij.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gzgtyllin.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/glwltbziw.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gxlnvxvvg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gsftshdyh.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gwngrdtln.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gytrsahqk.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gfklmnsxx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/ggcmlfehe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gpuokcgyo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gmlevbljf.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gpppjlrwz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/grkgtpdna.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gfihudmki.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/grvdtjtur.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gsfguwtgd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gjovjhwjr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gxgwgcxjr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gytsvabif.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/glbyonado.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/glpjbkinx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/ggnaoosoe.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gylczmzvt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gutuarehi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gofcjovaa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gvtzbuzxs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gvymvqbfl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gyozkcdwi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gjbhommyh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gdboraonl.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gwkiqxlcy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gnpxovhjf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gjvglykhg.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gebqesvkp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gezzjswfm.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gdfxwsixh.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gpltxaerc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gpbzucatk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gkrxxqxjd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gqmaqprbv.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/griunrffp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gicvqxwzo.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gdlninidy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/goofswaod.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/girfjfcxw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/greyvfybq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gesdexxxq.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gdcfaiwkk.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gvxzgiafh.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gfgwzowye.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gtjjvhrqu.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/goodretun.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gfuvvqdhn.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/grrtulbbj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/goteiwely.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gaqaefoqx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gcdnsoutq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/ghupteuse.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gjhshwewx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gckgheojm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghnkvoynp.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/ghgpmyxpu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcapnyyij.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/geerfesvc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gomxijdwy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gdjdusxmp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/guapuxxqo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gyojfhmfi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/ghrfbnlfq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gnmvrbtjt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gmrcgdqxx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gxroewvas.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gsmvukoqv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gnrrmycdn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gpttscwym.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gnpritjyo.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/ganuvakri.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gwxgbzkqq.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gsidrkudn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gvnzzgcsj.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gscfmccfr.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gluozsbmx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfeoixoro.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/ggwufhamz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/ginmkiqet.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gxyxkmzbe.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gtfktverl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gfvindqrt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gzyywwqsa.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gfigisyry.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gkxtpmnhz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gvbeyhnjd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gwamxdsfj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/giazkmgal.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gmoedcvhf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gscysvyxz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gupjbpeqb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/grznojcdn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gecwjsylg.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/ghdidxemo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gugtnzzdz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gtqzwwmcb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gywhxfxat.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gswlydkkr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/glqfajsom.sHtML


<!-- 参考信息 -->