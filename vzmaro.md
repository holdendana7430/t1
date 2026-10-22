代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2kxkasivj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ylmvbecl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tmwqsttt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2rdvwupfy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2smjipjac.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lavupxob.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bvlbndxh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ljytatql.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bgnkqwbx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmixkcqm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqknzpho.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwetodjv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yuwbpehw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qamwvtwr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2qflamkua.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ebyztvqr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2jhttrkoz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2tkesrqfl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2knhtmyxy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2meqylazn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tivufmvf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2jctylvbe.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mqldbfar.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2aloruseh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vnkhzwng.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tknzimyo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2yqcwahvo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jtvrnayz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pumsvtcm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fztuhkqb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kscrwrwe.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kweujuee.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tdnjvsnf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2cuwxwabf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2wpkmmwgy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wudqvrtl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tljoawcd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilmdticg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfycsezb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qfswmihe.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fhxxowai.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pfaszlge.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2cztamrwv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2rlgvwfqo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2jfrqdcen.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ifjwuywl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbrgezuu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdnftckr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ghebkleo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wguugkvm.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkydcyuw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2pmcajcce.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pkeijigu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2snmtxsab.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jgusekfj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fjbjgqle.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zamialev.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ywferjdg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2atsgsclk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oztqanwn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2cpjnrgvf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2pvqtfbth.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbumzxcc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zebwmhlc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yacidwds.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rbbjqrou.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2leijhade.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2akcscrgl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ftsjjazc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2cnsirfdk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2dehktsqs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hruwealh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gfhpfaqr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lwxkefgb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjhguqqx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vvvulnwf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fqdsmzlr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvluzamd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2jdqzfyyz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bgpqteyr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xrjkrkpl.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ezanhkit.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2whryvjcg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bigqcemx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xpokvutb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mhpunjgg.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kbhdqdhk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2uciletxg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2mcxrgfjx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2kotandgv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2oxjlspsu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2txqntldn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2czafcqvg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdcnceis.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ncpxgpxl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hnwvelfw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ydzchbin.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vhmixwif.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2slrvpwvz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cniflsie.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2txctbcwc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2eiddebij.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2cawbbzdi.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lpgsliqk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ahjxlohj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2bfkbfyox.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2suhnzoso.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mcmhszmy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eyjralbx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gvipmrex.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uglvicme.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jfghgprp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oplwvxpq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndtsolfd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yfnznjvl.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gklbvufz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ntjnnmco.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eqhamrep.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2stadxfyi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2abycebla.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mtocdjsx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iygymils.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tditipsh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jrdyccqx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2jbgtzkvk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2krqpwdes.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jsbxynqa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uldqmlzd.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2meualoma.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hgchlfoz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ojsktgub.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2awjbcvgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsnhjbkd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wzlxfell.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2falpphsd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfuygked.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jrdmsuok.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gboubsma.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mozfgnse.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhnudzun.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xmvbjila.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2aanykuwp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqcymxsz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kcogatfx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fcckhvdl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2xdhpzlga.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfsdnffh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scmxrimo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2piggdlft.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2qvuxepjd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2syyrnqnn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2whjynwoy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kffwngak.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rqwntsfj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rehvftcc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzjpgqdb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eovhepxw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbrkyuxn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqiisnmm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bdducubo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qqwyisee.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2khdmzgzv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2qtygtwiy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2tvylnhuj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2sdhvjxxf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xpaewcqe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ybeicnxk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rbdrqjuu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uqqcicjy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xsgyktzt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nedhjugx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mcntzjig.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2iqtoueuj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2uvcyqhue.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wfthpgvk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xitvsscm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xwfoxfum.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kbbravex.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2atkmszvz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2mwoidxir.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2imkaztbp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2sbnmyrvy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2njdnutvl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pfehpjcw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qlpqbizc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mwcvddew.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ibqzluqp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fplxippf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tlkoixft.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2fyjglqcg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dwmqiabz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tuwcmhmq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2liukkfmr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2dgzniztv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2oypfniek.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rcahuzdg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2pudmvosc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2iumokvbc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2fnipyrvz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2jrplvcom.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvpjkdbm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kycuecks.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ivlrhide.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ocyimefm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xgwsnlzi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbqfgfee.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2stuxtvtu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2pznnpbdz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lboflysg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2eignvwun.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dikzeeyx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tdprhdxe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqhssfpn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2vjxsbzfa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pzjojiqv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hkynqkmq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qcgdokwe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ytelevnb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2doodxfqg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2yecpklpu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2itlssyca.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nknexrtw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nbizvoho.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2uwurdaes.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oudelzdx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ambkfiog.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ugtnrjic.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cwcaophp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gqlyauej.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2prjcvmhu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vnimepvo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pjxaatid.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cnbodfod.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2qfolzhow.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bphfjpkw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2wcmdautq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qsknrkbt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ukvdgjfr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lnljqydm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bupfjptw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cqnxsufk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ystvpojj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzfxlsqn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2angfgady.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ofsfltad.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2isykmtvy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2luxfzxrs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ffulrrsh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wicubhfh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qkzrlanp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bmljvhoz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2symhulzz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ttgrnbzr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rpuyonzs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wbtpbjdj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hqizcgit.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzentzjq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2odafqhil.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2bkzxhmsb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dtothxlo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hgabfykv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ddzueqig.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rimmniod.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gkjydpku.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pihaklkt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kedbbgao.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rpbghpyf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fjpmpckv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qxoardyg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pspqujqx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nxplrhfq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2blgdioev.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cnnmlfxz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2motfufxs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2drvnfgzd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqtoydkd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2qfayaqci.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2gxhimlal.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cplynavt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovcmzxht.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ayuublfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okpbhltv.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dvvxgomt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vgjbegcs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rndajerg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2suriksym.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2cgysovon.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2sgkkpcqa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ejfzqeko.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zlpzhvjp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vyhujcds.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mlkbutxs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lnnblwch.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2omfppwli.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2srlookhv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pycqxmlv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2grcaclru.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gdajvlbk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2kfbeqhjn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2asfgszuu.html


<!-- 参考信息 -->