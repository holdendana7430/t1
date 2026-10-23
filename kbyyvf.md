代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ghcolrrr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jueocfig.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rfcshhtx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3cssezhpe.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3deperexq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yfxjfada.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3kucydgdx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bkhkfcms.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilgkggxh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fozemfvm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dqyvajtq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bqdleoes.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pjpqultn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3prlzmses.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3okqvlqtj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mmyjhkuj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3axvxiequ.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3akfbjrue.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnlzcjbu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qauhhomp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwpbhuxr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3yfxdgcps.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3kegguepf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxlqqnok.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zfpfueft.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3egmaqjoa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3szpfcnvo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xufkkdro.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ghcqenmd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3kxbrgycz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ndhqcwhl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3aphkwcvk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwfyfwgw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lksybtlq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3dksvbozk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3noxoozev.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jexgszvi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mxuhkxaf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3dlhzhpmn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zqgptaes.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tfzenqqo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnxqxvnn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3atapjeva.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3oxjxjqia.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jbogfggl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wyufqhyn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3foznqteq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3noieoclj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wbpfnkvl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3cbbggobk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oloiczdv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zouljqyo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3lcorovat.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jtyrcxkh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zqsythss.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3okrhtffx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3adzjqxqg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vhrhjahp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wohkdhdh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aciqjyde.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3psgynvyg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3hsxhehjy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaklquzx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wqhlpros.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xtyfcsto.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3tawiqlht.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3viqvgyvd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3yrthowlk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ihzbrmzc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wjxtfxzk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3dlpwsaac.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3mdmvuqpa.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3evuqiwvb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3zmxlqsac.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvgxsasb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xreioapq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3oiqcxlir.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wkhslrxy.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gowqntlr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qvqzldyl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3owmrkeon.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lfxsexvl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nfcsakle.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mknlnysk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3szlaxpbp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lonpnzsl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3pqpsswzb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nlcsujvf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3xxfgvyga.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ehuxveqk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ghpvffoi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kzsmebvt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3swklyjoz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3rgbuenkb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3qhnhxwzi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3ystxtkum.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3accvrkee.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ahotjvsi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zfllyycx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vweouihm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qntrncoy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3fzioablw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hcgljkuo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gwlkhkgk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3eynuibhi.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3oghgkbwr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3juirxjtr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3biljwqyb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qssiyqzh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mcngcayg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqeocztg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3aibkaxmj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3njofjwie.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xqxagper.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3zsjfrtyj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bikebpif.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3urywzgoa.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dyerjboh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nxjrrfyx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3clclxmnz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ivxqnwqp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ojwumahg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kebxmutv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nrmwppwg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ivxjzvor.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfnlwjjq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yhihdvgf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xjmhnkfs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zlyuotsr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ijtnwsnf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3snkorron.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ysbhamnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucyuoocu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3itdtceay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahkclmrz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tcbojtxo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wvkficfh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzipmjwu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmemjttk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vcrucybq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nqrdxmok.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3iklaxgxd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3nnrjpzil.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ajgpcmyu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mnnqujni.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3efxizvwu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdiffpi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svwprftq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dmbsnygy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3medlgiby.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3nrznppim.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yqkpxicd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3otrgduus.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3kyijacjw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3tkmfwjjr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjsdpdqi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3doaqptip.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3alqddian.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3zyflngek.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vzjbhbpc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mhjzmhdl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ptnghggv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3phctzfip.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cawyabcc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qkwnlqso.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3knrqstxi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mapnapju.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wheeoqeh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3noimdvpe.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfprogf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dqtrcjwz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3zvjpgfwm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nhohtvil.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fgemganf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3skieiquw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rxuhmmdu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nzruucoj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3raddbryy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fhgwindv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qkzqvmor.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sfxvvugc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ksiciist.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ypyeacuq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3szhjzxcv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uflpvtiv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dajrttax.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tchplglm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sfdjqxot.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vlvqcswb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3aajwwvwt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3zkxnkigl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vmcnromn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3weqxwzht.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3cyeblhms.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3njwilohq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bmxkvbaq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zjnjdrfq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jaeoxkcv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vvesshhm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kjwlgafg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3epwogjov.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmxhvppn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nvskomjz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3fmjopwfp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jnntznqm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3aomsdkah.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bpsoeycp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kpngrntr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfttczfp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssnzumok.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3btqfdaeo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3coznaysq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rjgahmch.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tfvyjlhr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwlkauvy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3atwohyei.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uprbhssr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3njvsxtvt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3armogspm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3zbkbvbbn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dgsaqcsl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yaapnvnd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xccwwcml.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3brioiumr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mrepefyl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3nijctvvr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hrklytxo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3azlfxcdw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qcawibto.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3kwizuffe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ikubjudx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3sosdiriy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zjxsmnbp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3suyxgzfi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wksmhgzl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wpmmsbcv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3bxvgaprm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fgvzbfnv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lihjvaaw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zxakhvxk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kbcrqdks.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3qdrlpqxo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3jrrppuig.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3uzerrwte.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3efnlvzvq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zweeuzjr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pvumykas.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fppljanv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kijqjrtk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bbzhembs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3qmijghco.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mjzslxwm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3iujzpjza.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ifmoexaz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jnlycjso.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mofxiatp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzfgwmti.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdbgvwto.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3cvtbkmlt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3izxftylc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wfhuwyns.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zrfquzyf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gikzqzlq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dwsqkixl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzinqfwr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3isvzzgnv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yoenhzbl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wokxybpv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3tbgtoegh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3abqahclj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bgboezpj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zxzlfdvg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fjtbnbyi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zaohukul.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tubcaffq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3puvmyljw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3gbqrrnvn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pgphhsmq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqrbvrqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aibzatqe.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3remrjoif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmryvzbm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zfcwqzjg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mcxafxys.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ixhiiypy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tjjzdboh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qzyeowyv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3mwbigehc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3eovcjoqt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3oooakbbr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3gmjpserh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3yfgixeuu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ubxgzszp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pojaasjl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bsvrbbft.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bqvutkgh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3aqenqyar.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gexnjsks.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pfvkwmgn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rebhwdvo.html


<!-- 参考信息 -->