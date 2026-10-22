代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jizopmed.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lcvjbunc.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsmtfzpg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvcaeyvf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2gfcwcxgp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2zljpnxqw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hoghcxxn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wusypdey.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ocnfdpio.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2whaknorw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fwlwyidj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2slrpktls.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zssdjoxv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zgcyibis.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mtmreeyw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2gafmdhsh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sehcgwid.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jqdhgblr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmrcfgiz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvlmxguj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydlnfizr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2tfcyujye.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ujnnanpv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2isctoosn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvfigehd.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vqqxwsbj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2oecomqjg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsoxloxz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjerbgix.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2netwcocu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2dtexotmd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2avnfgnwg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2inwexndw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjrwbnvf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vciblvrr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2eoklowxf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdvqvujm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bducjynv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzxikoyz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aelbgjcn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xektnwld.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2lypbvrdb.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bbccclhy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2mhjzgkdi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lcxqhekn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cyrojkaw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2icdkihft.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rqzakkrj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jffvgpti.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nyawsxpw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2mixipdju.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hlkzftkf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2geqxhuwz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2dyofdczo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rajtynvy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kpkxpgns.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vgozqljy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tratqzwe.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2qoeobnef.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xsrywdyt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzybnxir.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2bihuaeqr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2thnudwyw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvvgsfrv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cwfihfbb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2rpwhmuhi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dtwdxayg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2oupcfyxh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bkqmslul.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdpoxzsw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2wdhkvyqx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vdwwjqmk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xnaxtfwm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dscfuqtb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kmflkrlz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2egykijli.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2erzttcwi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mibhsrfp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2apjyyufk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zhkchjbv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2upoywvcp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ktkqetrm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2dcdurxxl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ffmwzbjw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2esjdpxmu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vwinuwsk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2dqcpuicd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vyfsfirn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2brdnkydj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jfolrrgj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtflgyml.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2igltyqey.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfjkhbur.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ujxcvzzr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2obwsknto.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qsteiaqn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2gtjbalfe.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2kpxtisjj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2sfbwhblc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2blqdmnsm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hdqzxaiy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fwrretgv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2agwoscaf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2lfckfmkf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2szqmyisz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tepgsllf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2lmuqxdod.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2pewjeolh.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2svcnhmzy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xkcmdxnc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2goqjgebo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mjtifqso.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aeejsspn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xgbohiyi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rxwhxzjw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kblzfcoq.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2gelyiyty.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdomspkw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2pzbpylzo.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ukxukpjf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2swrokrvx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fythlmif.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ncjpvwsk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zusgddbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldtyfifb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2icmjmwhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chozoulp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2smdephyx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vxxbwstu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ygtgxwsc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iqknwtms.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2avkisowj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2auoylupw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mpyweklk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2kxpcpovp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfcwkozg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kcremhzp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ztknoxxi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kqokrfnj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cjledoeg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vqhqnrmx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ojtvqhfl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ockixejl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vooupnyy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ziyzujue.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2btvfpqqk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2risuwudx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wadiyxtc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pcpqmesl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2aumfjtwi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2irunzqsf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wjwlmmcr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2gttzuwmf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ungnpohr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2noibufcg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2xrtkvrjv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2buichibw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wxugcbwx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gqtvixob.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qayzfyjd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2yocilduq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kapprnfq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2shggmypu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2evezlfmy.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2inkeupyx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kccyspkz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iuuccjoi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xmbheqsu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ourgjhzw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vbwqmegq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2dieqqzcl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ftyhsxkh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tptvetry.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2iodblynh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xveqyszu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vaorildm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dmvchxlp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2dkdkdlsw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zlakyxtl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wkytrach.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qamzybeo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2zrykdzqb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2csapnjbh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zbfgleqg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2uvmrsruk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2yvbmcokw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tgjcvdzo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rncnxfgd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2eosrnfca.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2mznlardc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wsylhwqh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2uoqhztcp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlgarndi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rgaseswk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyvqdvyr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2shcjfbpc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2muhnvayx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzlssrcb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ykaukqar.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2aentywzl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhmafrma.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmfhelew.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bxadscdt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bzfucuis.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ondnxzyt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wgsjykyi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wrmyvgtf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ukvzfngw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lqmydvks.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2wgkvmndn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2cyxdkubl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xeemtpdv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2shfgpttv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jdgswsys.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fpwdvmnk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2yzoylnyk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2crswwonb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2eloqdiil.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2mzuruvfv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ukanylol.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kwdejxas.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2evcyyben.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hkrtdewv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2tocxcwkx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rqsdnnpq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2bejdknwc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zprymggm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jmrguvsc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2saogtkue.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wbmvebmv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jgeeaasb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2pbnxekwx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ffhkeqsx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2njujiuil.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jdgbgxzn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cwpnioog.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zmeiqcjn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmyutjqq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2cfqxsrcu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lqjyiuyh.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cfseivza.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2jbnwdrko.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ccsdoxea.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ctasapdm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ublmuakv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2doddxsdh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2msycctwg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qyjumcqj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rhczzlyk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qiwzufbn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ltjtwxvr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tpbbutbp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2amytcmrj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ileqtqll.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2zfztmjvf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2iqeevmpf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etjwnbjs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdwwrnhg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cvjsupvc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rjjyspxh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2satvyczz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lhumtpla.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kikenuti.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ivczexth.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2sdrnpvge.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2cttjbzwx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hkhcctdg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovnixtrb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2blkevnhh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2inbjujcb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbnfnsth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2harospvh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2sehlrvcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljbeydez.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nfssotze.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hohycddu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2arokghvn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ebfgommo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ycjxiuep.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2haahasrq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ryjrlbzk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dcjkuvgd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2gkfxruar.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2azwzludj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jwzyjzmh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pzcowvoc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ynquhamv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ofcrtvyy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ereokdum.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2fowlglek.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tulepfmd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uprvmmwm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jxhxyupd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mwfmxljw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2hyggpgkk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2agklgeeb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2crwtcmkz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mpdluvsc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2anebpkza.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2psxvevqj.html


<!-- 参考信息 -->