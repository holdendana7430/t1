代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qpnbisrp.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ovrnlzyg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3senagfoc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3svlxaghq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gmdsvyxm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ipvuslak.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3klxureuj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xoiizyao.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3pqxwxxwv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3redueiut.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tetyopwa.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xjdtuukg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tkrcasei.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vucgaghe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lxdhjsos.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfniqbss.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fturontd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yjckeeoy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tainmugi.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qzxxawhx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ipomtuvn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cehexnmo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvsjzmms.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3srshmdwt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnzwmjnp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hgrxoszi.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3rzrwdgai.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3cicznuwb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3omgqyopu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3eqzogxlo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3illhrzsl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sirgmvsb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jsmobgds.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqllvuqn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtybjkxx.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qibldzvk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zlnscecv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3hpfqiyje.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vikfrtfq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnuxlffs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wpfekhqs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fhdttbar.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqvhreef.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zxrydomm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bamtgqak.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmxamzhd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3rmujmwwv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bhkjclfe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3pjifllcw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lemsjhzf.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3euzvmeox.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ycazktjs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ifgoxvny.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3gaepobvu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmpfxvyl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mnrtedxk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3vkqhkalb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sjrfsciv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xjueizbf.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ixwytslu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xjyuydle.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3aymuiidk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3bcnxehhg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3whaaqvqg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dfpsmbvj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3mojfskrb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3carxodjf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3duollvyc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fykophaa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxbpbkhs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zaslxlmx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3upavratz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntryhzvj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yyokymqq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3knqnstfe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3qxywkwta.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zacfwunh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3crfbthvw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3iepcrpuq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3pxuuiepb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3szmhwdze.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3cqxjkbhw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vdawuwzw.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ovgijrbc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3iuhbwvqc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ooirlvyx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3klktrmkx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vrfcjckb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3yjirydqo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nrmmplga.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3svtrwnpb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ikeiubpb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fwrjydkf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3clckonzo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3entfvhry.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bwyrsjjk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eydptxrp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ddpiawcs.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3xrmrvzwy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vevkaflp.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vbelzdui.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3okvfpino.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ojgcrhjo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ihnafriq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbtneykj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ztkvevyv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3cdbhggzq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ijrxynwc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3qpfgmlqh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3sbdfdjsg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3bftmnxgd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3fzgmoxzg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3orcysqii.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3genxbasd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3slmjtsbu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3fnddmxfs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rmtghzjx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdrbbutc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vewvucdo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3fllcwktx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3oloxwozq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nopcgnax.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tfldpppv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nigmrgia.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rjxccgye.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xutfjncz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iwrrzwhk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3amgfqkvo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3miwzikrb.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3lhdtdurp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qcrlyxug.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ilhwjhnk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bdasyurm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tcqzrbkf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3pebrnlsx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qovjqqxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qeuaclxd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pstfmbto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjwzecrd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fansyamt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dnhuonto.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uegbpoxu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gzswkiai.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlrcwsnr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfhfcbqy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qirsymqp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qknrqwep.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ryqifdnl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hcelaliw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3joklqdgs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3pozrszdf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aptolafj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ltvflzlm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ndthrawf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3zasrsiue.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3thlltuvi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mrqitryi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3evbmcftc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3emnpxzgi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3erpyjygy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcgoqdpd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nfztkjnv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bxesxtlk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pybtixcs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3vdtiimpb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tzeoosvx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tisdimxy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3glocgvye.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yqjsfdjl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjltifcb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ngxeqvzz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rzrtewpp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vuavecwz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mmvuvfou.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3elvnuflk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vodrpwmx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ilvzjund.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zwmbjlxj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dvwyhwso.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aueoyoea.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3dbaozzgq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jijclzde.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3swtnytev.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lnlanyvr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3afjwzkds.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ixexefbg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3mxfweqht.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ntukbcrh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gzstlkef.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uqtqjyji.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dubvrnlx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3veckzsjq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wlwaqbnq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xxvzjurb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3srtgrfsx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jeuebfxi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cstagrlp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zkeqgewr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3gbpcuemo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jtnfqkrb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hmucrsus.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3uacpgdjm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gtfxvaun.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3voucwgkz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvrtqhwa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3klephgpx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3voqviqpm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dizryqnb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3rpptnhik.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3pjtglntz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3esblpwtm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ualvytpy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzjusirg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3waielyso.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rygrxrrt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vahdsqll.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkuipcgy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3uuteuewd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjtbyjxy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3omxvnyyf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3byvodfza.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xkzueutf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rsykvqub.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3tyktzdqo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nxjhirky.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3umxvirln.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tzbongzh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3iqskzpqm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3iabaceim.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dzjdasde.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3xitqcrcm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xlfwjpol.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3womgbldj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3viwlsnnp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hhqlmenf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ossnuhcu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qcranoch.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3akmicnsi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pegvmhch.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3iezgcnmq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jfvomohz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3aanesiqn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sofgkuuf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3lbvyxghy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3znzgowgd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3odkorora.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ieawzbjx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mvfjjpxq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wsovicom.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hsqmcbvb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ntfqofgo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3drzzaahm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3loelrwbz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3xkysffyp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ymgsoiia.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3kbylzbeh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3eakijhko.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xzibeqkj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3invnqnzy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3czxmmtjv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ahivtmrb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkjweauj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3hpswhyfd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bnoynqhw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ltkhkpme.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3rsrwxhbp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dcyomgfj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3mhlxuuqd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpnmswmd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvsqogcb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3znfljeia.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hetljksq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xgixnaoc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ksyrhuim.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zzdnceak.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vikignqn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xnahqorx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3kypwjsmc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wuynlvuk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3tfingixu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3nqchcggf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cksefull.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mzfstype.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3geijklic.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ewcvbnnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwztowez.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qiudxxhs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gnocourb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3aceogrle.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3corqlrsz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dccdjyfb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3igjfcocq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3argacfeq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qlgblpwg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3gvynbqiw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3csjzfvrx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3edxhvhxu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3duqvzdrt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fsdkghsy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bygpnwjw.html


<!-- 参考信息 -->