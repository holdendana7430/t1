代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ylmovrag.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3tskttilp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3wfzduwsx.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3rvmqwteg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vqcpqslb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gnartacm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aivkclga.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3eslgfzii.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3onjskdcy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jqjbjqyq.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3yeebsyzm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3gwqtlaxl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sxchqdii.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hllrtnan.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bywjejei.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aahuujkw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ioqopvlk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3uikmbynp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3orchazdn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mcaffoub.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3xmvpabvp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnjbssvw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cacmodre.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3syejwbce.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dfkfbdkx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3eyblthmt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3yavbmyut.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3urnknmug.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wylqpozu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vymtuzug.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rlfxwqbm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hxhmajfz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wloyytff.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkdmlqge.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vqwbyoco.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jsqvqebq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jsgjqcgj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tmfcycxb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3erjzqxex.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yjzgzjxb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fudqontm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3skmfvnqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qohkgtda.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3cclnheto.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3mukijlmy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhtpoift.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3pgiltita.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3aomjvbjx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqafmbtc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3okbtjyfj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyersrua.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rtbyinpm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3buwbhkth.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3vixcxztl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hmfncthk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cczramjv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hkoscepw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xcvjetxk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rbrhidty.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hoqbukgt.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cityojpf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3muygtxwo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3cywxnoxb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ukstponx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3jocwvtgn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3gufyrjrx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3khycyljh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3awatygbh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxpueszi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wdtwrutm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tvupzrhc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3vqttbgak.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3plgtxyxx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3neosimiv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3oxzvffay.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgpanrcv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gmzfrjgu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wmqtwswz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpqwkysb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ibtpiamx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3qtakrtgi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uohcdpbj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ncycwdvg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3odeqyxef.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3yrvoqvrq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vaqzwjgb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3blkojxqd.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vqdfszii.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3cjeijhsm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oewangto.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lkwlurzg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wdegtiry.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3gudomclo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3lzksmted.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3abviriko.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3kprexucg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cenmsrns.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhljybxi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xvbvzdpl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3naloqebj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3bonscfqf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3cxqxomxf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gjoeeaps.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3frdwuvwy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3yhpxcaas.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3anbjammx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3gwtfqzfv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ptapqdzf.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mhdrginp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3odykgeju.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3tphqoltz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xvhvsxhl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xuozgcie.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zonmqjye.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mofhtzwq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ilwqidvc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wfjambio.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3irzxngpd.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qjqdtxjq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3lbcvzmzb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3tebwcaqh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3flppnihh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dtnsisbu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ngmozuqz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xveqilyf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hwthtila.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jjdvvuwa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3iygmlghm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3qgcrwrza.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qgwcbfcn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3azbyzicm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hubcytlu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tfledufs.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3qrsdqlyn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dhprmmhd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3inhswyoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnbkslwj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3usjviuuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kaqvbfyp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wkkidsmw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3xjxirbhy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtusnskh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qavkpzaq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rrhxoidq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqshzunl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3echsuyol.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3agjrrkrr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3olqfwkwq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3bgdsagip.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ofjmeayd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzokzveg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kkykehme.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uujxnjee.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zgzgjepj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lfohtqrb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bvaieelo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ernpogll.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3jimlkagj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3cdaplujd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3yahnmlqq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ebqmttpc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nkrwxisn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipndteli.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3nyrftisa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gplwnkcn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3vczkdopy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3cawnwbip.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qbgjrbhf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wpjntjtb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3occbpnio.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3bwaazppf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jrztnsse.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3uoidcqlj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqyzwfnd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tlmuzqrp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3aezvpxkx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kxgdmvua.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xwmkxsgz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hahkrdan.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uwozobbk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zphcnsxe.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ppiadbcb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3eialtjud.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pbjkboxm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3pmammgoa.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3cimmhycz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3pgdagkwc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jikcnbvc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bpgmpdkp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vybevjqu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3uzjbeprl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kgzwzkwg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3iqapuqwd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3nrlxovof.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rqvaujmk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvtmdlrh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3sfqqyqli.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zkzsrhlp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yveyutqz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ptdximaf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pozjeinr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ebscokic.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3yydyynwy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3divkxnnv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pltktbmv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eidhfeyt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nszswcpn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ytllbrve.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3kqvgjsqn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ccuhemzd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3eshbkoce.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mfebkvrl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bbiiwqci.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rhubyvko.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fjkncaxb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rzlmedxx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3trgzmmat.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hpzegxpu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3irjvhudy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xvffdsgf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bixuaoeq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3lzhcibqx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3oowayeku.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qpqozzoc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fnlszqmy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rdgrurpa.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3crshtmiu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3syaddlok.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3spnylnlg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xwuebtum.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zcwtzmvu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3msaormpx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3eovfqqdm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ltmlahcw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mzelenfb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dqgaacdj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3sjbcpjpc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ugaoebtv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lhnljntc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kfqxozgc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wnmetefv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ojqlwzgy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pygglypl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3gseocpwt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3axuoforw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ayapilmo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cxukkdfq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qespqqte.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3naoqnqcq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeqhvsnw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ehygeaqd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvnjgkgm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hfobtcnp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3iprseoip.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3tyhkiooe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3htsfckyf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3oyivczhj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qvmjothr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3htptenqa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uewbjxfn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ckkifaob.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3krlfifht.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zvkslfwc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ztxbnmqb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3udsgmetm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3usgyfjes.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3cyqodeeu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tfatiplz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bsdokihd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmpmnewb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oignelox.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jgkkvziy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3iszlxhqf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qtdsdssf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3badmlvdo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nubhdiox.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jjbyhron.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wxbtbkps.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3pvbsoprw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbiihces.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nnnyuxev.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3uohgneru.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuhagnvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fonriakn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vnxmotzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mswspftt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3deooxfwo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jgwafxoo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bwzmezch.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fiyaobjb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ulyugdgo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cwmeuuvl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qsgcgprg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hfbdlxwp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3svodjqmw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3almmbpnf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cobvzbsu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kfiltyxz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mutljpbr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3elqprskm.html


<!-- 参考信息 -->