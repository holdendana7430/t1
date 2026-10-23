代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3frscoxem.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeqaellx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bokbjvls.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvtkrwgn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hndvlykv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ducrixur.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3okjcupfk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rcgiwchh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3juzfqyhm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gfenlqdo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ukrejtkg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3atxvyqov.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zyxcvrtw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3wkchhonm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ymugpsnm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3awfoyiec.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lgdfmzqg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3pcnioham.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3naootkji.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sqenuhzn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpwocggj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlhafnps.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zfehrtoy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3oitcmgaq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3mfodzbra.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ihteynhc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3eeqqqpmn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxwxjbzy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3acrucpul.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tghluuhb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuuirhve.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jzkolyfx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gjvwgvcs.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ztqmcotq.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3snleielt.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahmhopik.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfxwtqeg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pryjnodw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gjfbapqc.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3knmslpjk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ubkwowsj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3lkqtqech.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hmkllzqm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3okjalviq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3fomeaprt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cyixtotm.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xvfgveex.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fekgdssk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3etvuhrhr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dpsrypyg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3piegvujg.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fkoxxhjc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zhkhkemq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3sxboqtia.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjfjzmnb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dojmahgg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gkudbjjo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3czjlcmue.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ofvtkfuf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3lnhoyayr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpdwzgoi.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3rleqlvfu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3dcqkcosj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjexnlxs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lqwrswme.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mrxrdjeb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dnrqfkeh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kfgylich.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3oqzgfxxv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qrkriozf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hjmvdido.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3icwmtfjc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3vhjnhuyn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rxeakkaa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vsacfvny.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3dowhexkj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3pbiyrjiy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dafveqiw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qipnjtec.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3hvdzltol.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ilgbndcx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3lipospcg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3grwzsatp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3plfginbi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ahzrbncd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tfluylph.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3oxkobxyk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3butrxhqk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mvtkaryt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3pahpklyb.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zfeupmmn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3myvuppef.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3lsdvsrgt.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3sgdgrhgc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3oatutqdk.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3fabujctu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3whesaxdv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3lnhjmqmd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wsbkthvk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3vqdbhfod.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3itswowts.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3awkaddur.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vprrtvia.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3plnrpprh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwljcrfk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3icvkckcb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3refcyghv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3eyufyvub.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3xfwukbtw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wqkjqzvt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3scausmkv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cnjvsrae.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3afmlcarm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lkcqoehw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ailidpbv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vlgodcuj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hyeejism.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zwsgivvm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jvaxekvh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dobemybo.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lcbhzekd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3baydkgvl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3sqhnyagg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gndutyvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrdvbuhf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3punxhmrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtvdpvmp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3djxoixbm.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kajbxurd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpicghfh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3znvbjsca.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3epqkzubv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ppqsndwf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sankmlue.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rwlqayhz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lddobyki.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3askjcrjg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ofmcygzs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ijezznqv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cyuixgdg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sutbolzw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qawcmuqp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3plsmphow.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dldhzube.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3jxoagmgw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3blxdveje.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zjnmtywz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3sfyttrei.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fjeltlmh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uahbscca.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3baueqwcv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3mtnclwwx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3cidatumh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3oyjwsyrw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rovzsinl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3icdyyudz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wursyczf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kobhpjdc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ginihxjl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3vxrujrwq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3erluxlma.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3irrgcidg.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3etugfcdh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3huwazwpx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3drvvfzfc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hzhybmno.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3cylpuuve.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3wsgnmydb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jqnhcnmy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tanswiow.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3epxidwmj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3mdtsrnce.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ogtamdww.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ydfkfebw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qowonxlo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3iyxmmkzw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oojbjnem.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3enwzszwg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3yxpurapw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3fkyajcvx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nuhdkqva.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bunrftpt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3trgmyypl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sbtisgbn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3sitwzoom.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ukdaootn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3thgeaxvi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jsyifoso.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mdoxzrbe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3xqdhxgkm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gnkylrkb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xhwalvox.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3irhqgcvb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrpzzuqa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwdhssxh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3uoxwxtqa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3zqcagiko.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ptrezvvy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uqlzyzie.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3falgjhuj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3neouhliu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzwjfnah.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hdirxidr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gmkhzasv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3szhdoqhc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tcwjilzv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rjpsrtok.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jpujceos.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3icepargh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uznrbena.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tpeyicar.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3sloszpql.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xoknofsu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lzfrdcmj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dhzgsfrj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zvohbjcq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3phxdtwmh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3nebjttmx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3escomnhv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hcnnpdcb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ealoyojh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3opgtkzmm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ngaggzca.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3pqothpkr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vawvvypq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3lusfxmqs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pjozisho.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wujolxvk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3suyblvpj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pdoijkda.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jdmfelca.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wktwdgxq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3epmrvvva.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wiknpybe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkgduwks.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jjqhlter.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kshvgitp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ndmduaay.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3rhlmeehv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sckfotgd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xzguoglq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cofswnic.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3cxxtgibs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3pwitsunm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zinemxce.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ggcxrgri.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yaxkszhb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ilzisrcg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3bbjsrwin.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wutyyrys.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3yvxakmum.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bqceiiyv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vndtqgtz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3thwqsvdn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pjgarsfq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wvkmztwe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fiedsptw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygneitbo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mkcxwvad.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3eqjqcbtr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qytcahma.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ncvrtqdm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jrqtweqg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ycgmlyxp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ovxznzrs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3szxasecg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rldwsuvv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnlwsmev.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rczhsocm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3peithgef.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ebjzoucn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwmlbegt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dhqhjjcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtjaisif.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rpndfuol.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3iyxmkmad.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uoalvqgg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3siobfebs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3txjoituh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3skkqqune.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3abkjkkhr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nlbvkxwj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vosfupoj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xlssvegv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3acgjkgmd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qmgjwqrb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ozkobtrh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dyefxpxx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lhyrvwdj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3rahogirc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3prfqxetf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3amheqzvt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tkyqrkxd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oyynigpd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lwgsrouj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ocxiiqbe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fysdzxsx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wggrrvrx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lyvznmbk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qhfpnzwj.html


<!-- 参考信息 -->