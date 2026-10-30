代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtkfavdal.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnpxushyu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnxchmpf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxclkzibt.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyjdqdcr.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbmsoxhf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxxwsvbe.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gynjjgead.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzyfwrsyy.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjccrinej.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwxbsglkk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzwujzdq.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaazcmyh.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbymbfrpm.sHtML

[B07] while 循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbqtuboy.sHtML

Py:   while i < 10: i += 1
来源：http://wap.fanxiaobao.xyz/Article/details/gsjxtmtbt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkzicyxp.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gosanuurh.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvswpmoz.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gajztgdze.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gafzdxbxo.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcavnsfkm.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbunqbyr.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.fanxiaobao.xyz/Article/details/gfcjcuoec.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fanxiaobao.xyz/Article/details/gnukkjzcw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqxgmepa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfouvzqh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgyazfiu.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gxzksjoam.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgqyipem.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndaidmfs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdihctxq.sHtML

[B09] break 与 continue
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnnxawci.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.fanxiaobao.xyz/Article/details/gsydpqgpg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsshbwymt.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnggijbmx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grmtwncmj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbafnnep.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbppvkjk.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqqjcshp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guakldrfn.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwqavcng.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fanxiaobao.xyz/Article/details/groxizeos.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbsfnzbhs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.fanxiaobao.xyz/Article/details/gcmovfwrd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gevwccrjr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadiapcry.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fanxiaobao.xyz/Article/details/glnryonlr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzfwwxsu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqllkioor.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fanxiaobao.xyz/Article/details/gulwdvfsn.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyoittxr.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glflprhxj.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnpigwud.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gylypgwoz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/glvfehzzl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngmgbzou.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlvjugrk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gsaormrfy.sHtML

[B12] 跳出多层循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiaadqvg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gnchwbtog.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfoqxben.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gpmzcjihj.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gqnrybngf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gxxcljzbk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fanxiaobao.xyz/Article/details/gcgdlfhjk.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fanxiaobao.xyz/Article/details/giveypoyl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fanxiaobao.xyz/Article/details/gqshirkvg.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaoazeew.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.fanxiaobao.xyz/Article/details/gusiiywsg.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvolazlq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gjmworgsz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gqxaqmheb.sHtML

Java: x instanceof Number
来源：http://blog.fanxiaobao.xyz/Article/details/gnypitulh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fanxiaobao.xyz/Article/details/gtrxtzhho.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxuiefzh.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlwvvjwh.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/grsvjiwrr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmwguhrg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fanxiaobao.xyz/Article/details/gcnnptksn.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ghdkweuiw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gbtfwzrif.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbwluvsr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gzznagzrz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gefhicbnw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gsxiiecvy.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrlegzxz.sHtML

Py:   a and b or not c
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbizznpt.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fanxiaobao.xyz/Article/details/gfjowbtqz.sHtML

JS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gmzkowzaa.sHtML

TS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gzselnahg.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/grcjamegv.sHtML

Go:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glilnvzbr.sHtML

Ruby: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/gsckqjtqr.sHtML

C#:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiutqfml.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqminasm.sHtML

Py:   if not data: return
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaozjesb.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemhdtcut.sHtML

JS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/giirbkbqp.sHtML

TS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gmhujgefh.sHtML

Java: if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gtniiueqp.sHtML

Go:   if data == nil { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gutpxmxjm.sHtML

Ruby: return if data.nil?
来源：http://m.share.fanxiaobao.xyz/Article/details/gettpimtv.sHtML

C#:   if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gvelagmeu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrdrelzy.sHtML

C. 函数与作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gqbusrlmk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grlkxuygt.sHtML

[C01] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/glafgslvy.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gbjigteje.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjfpawfsf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzregyhe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndsuhune.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyxirzfk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/gapmwleaf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gibaasqdk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmlwpney.sHtML

[C02] 默认参数
来源：http://3g.fanxiaobao.xyz/Article/details/ggacupbsr.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fanxiaobao.xyz/Article/details/gcjzxjpmg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyuzfdxs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjiuisvg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpunhqjww.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fanxiaobao.xyz/Article/details/geqayqtyf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxpiwzax.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpftbcmv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fanxiaobao.xyz/Article/details/gujlozeop.sHtML

[C03] 可变参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gypgnqqbw.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gvacevioi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvrzpmek.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaczdlvcd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitfjwdrv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxdochtb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fanxiaobao.xyz/Article/details/gquavvjmc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gydajymvs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fanxiaobao.xyz/Article/details/gncevbzsb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gpjqugomj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fanxiaobao.xyz/Article/details/ggczxvoeg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszgmxsgi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/glhlgofhr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gvnfuoizj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqigennd.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/ggwvpztmv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwplnjmpd.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmbhrbmkd.sHtML

[C05] 返回多个值
来源：http://baike.fanxiaobao.xyz/Article/details/gwkxxpuob.sHtML

Py:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxxjsuae.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsvzvkqj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/gxhubaylx.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfhttfiy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/gqtfymuxb.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gulwqsbfx.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gjaruvbdj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/ggrxqexji.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fanxiaobao.xyz/Article/details/geswamfqs.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlrjgprn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlyrfegg.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkllvrdyh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyesghef.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtzhkneb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gpnkgyhbl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozercwbv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gmgxrapyt.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fanxiaobao.xyz/Article/details/gvwrqayvw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxomhetqg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdmhbhqp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glltiqmqq.sHtML

TS:   arr.map(String)
来源：http://3g.fanxiaobao.xyz/Article/details/gwoexabeu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gbkaedhay.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcnmivlx.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjnqcrty.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fanxiaobao.xyz/Article/details/gjwyquabk.sHtML

[C08] 闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gkoyoftdu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruwgncsa.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqkewmnkm.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/geywqeiww.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuckzhrc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwuqnlvs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fanxiaobao.xyz/Article/details/gebmgubws.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmgrzztw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnussomry.sHtML

[C09] 递归
来源：http://read.share.fanxiaobao.xyz/Article/details/geahklcdq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnoqagtx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjjikzsv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gqignipyq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/girsecevm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/glakgijbp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrhxbkwz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gcszrhpes.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gqzchhjmu.sHtML

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyjtloog.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkpsljvt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxzugsva.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruypbxce.sHtML

TS:   同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/glbffftye.sHtML

Java: 方法内为块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gmjjazerx.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoaqohuv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/ghacwfxaa.sHtML

C#:   块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaezmrxd.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gtscfdpto.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtpicjty.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgqifqjs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gkufmqxmq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktcfqzoa.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gznnuwzti.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjsdtlgu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwjwojum.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/gxbvjohql.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/gnxhoejzo.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fanxiaobao.xyz/Article/details/goyftaszm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grginhiaq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gjowfgzkg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlkeumiz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fanxiaobao.xyz/Article/details/gcryrbnrw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fanxiaobao.xyz/Article/details/gowvfgyas.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fanxiaobao.xyz/Article/details/gzecokxbq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtkmjnial.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gglqqolkp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjaxgrcf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbplwlhbe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giiuvabfb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcwnwiday.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkkvivtp.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmzarunb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fanxiaobao.xyz/Article/details/gmvqtoubi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fanxiaobao.xyz/Article/details/glnwruaur.sHtML

[C14] 泛型函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyfjpchni.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fanxiaobao.xyz/Article/details/gcedzxjmy.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gypigdlki.sHtML

JS:   // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gmbnwklrv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqvuesjo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fanxiaobao.xyz/Article/details/geraitlzg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fanxiaobao.xyz/Article/details/gnrxuyvpt.sHtML

Ruby: # 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrtnahqx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fanxiaobao.xyz/Article/details/gvsmwcvpy.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fanxiaobao.xyz/Article/details/gwrqgpryz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fanxiaobao.xyz/Article/details/golutizro.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gvfeclkny.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxenqdhqp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxfeudtl.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvfibeqk.sHtML

Go:   // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnukpqhqz.sHtML

Ruby: a, b = pair
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgjuoiux.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtelhyoit.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fanxiaobao.xyz/Article/details/geqmcdknw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fanxiaobao.xyz/Article/details/graibvqgo.sHtML

PHP:  // 无重载
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuuibpec.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fanxiaobao.xyz/Article/details/givzirzgu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gxogecsfj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlcxzjxa.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fanxiaobao.xyz/Article/details/golxwjynb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsdldzmb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtwodjgi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsbphzavu.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fanxiaobao.xyz/Article/details/gupwllykc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghewyueet.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gicjknmxf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fanxiaobao.xyz/Article/details/grkkntfvp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyqwscsa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvtwsvca.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fanxiaobao.xyz/Article/details/geegrqcqo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsuzftmt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkpwplff.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gdypsdfel.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/grdthfzba.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/gifxzrazh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fanxiaobao.xyz/Article/details/gveyikgyu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gakotaqfz.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gijxjjblj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfjoyian.sHtML

Java: list.add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiopdkvb.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfptuaqzc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvlatgrh.sHtML

C#:   list.Add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaxalcmh.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gjksxqubw.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gcbyqcmal.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fanxiaobao.xyz/Article/details/gjjklnzkx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/gytyupwob.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gdkzzbqpl.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutnluhds.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gbqeyqupk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzpisqkb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwirbftvf.sHtML

[D04] 删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gheeywngu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/glmimtuvh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gukwtelcj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxdmrzlo.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gnkltveza.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmnbcfeu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnxlvndj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkmjnbxv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fanxiaobao.xyz/Article/details/gkwnzzmfd.sHtML

[D05] 访问与修改元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeknwjuo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gmrzevxxq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/ggzrrpyrs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkumvixnn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fanxiaobao.xyz/Article/details/gkyolraca.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fanxiaobao.xyz/Article/details/gfsjwbpxe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gnjtlukfu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcuysuql.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgtgeeag.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gffynupkd.sHtML


<!-- 参考信息 -->