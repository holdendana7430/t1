代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbkrfkaj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmtslonb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xvhuzvhk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kmytvyvj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3liwkdmxf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3apnfvgud.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pkdmimxk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3spdtlamw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3isqbaypw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3flnlslbj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqfkrkbh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3teqamdsl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbnsmwej.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tzilrbdr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3alkxxjri.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3owexkagz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fksrysee.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3luvvkipk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3etwmhmlc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3drnquupb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwtbqkbl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rffgrmwq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yfmetyuf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3dvxdmpyp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmzbqzar.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3bpplwtln.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vbclgqdg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3jgxswlti.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmntykox.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tzyyllqj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qddmjgay.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3bxxiikfp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fkuqrmvr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppxldvtz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ofplegol.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3xtefikbq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3csjnwdtp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qyjebwsi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngaljgzs.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lnnpdqco.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mfxyumld.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3urlmgxqk.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrdiburo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3jyougrth.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3sqmfvblt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qkkvdbqu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pfbblimi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nxhuorxr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bzoopdvo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jviggvjh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3htecfqtx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gqialbtv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qiotzion.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3zidmamlm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwngxadl.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ragkgknt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3itiqbsgf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3limsrnjh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mmmnngtc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cibuftrp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3amkhhvuv.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3eulokowc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3mbefeobg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoxwtwco.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yjtouiry.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3jrpkqhnz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqbewape.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3svvmuiqo.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zmjcwlxd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3splkigsq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nddessay.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3auttkcfk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3liwiqmqm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mafyaakq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3godfceqo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fklqyhgx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ngsyrlvs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oeowwikp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3luwkblih.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3gapxclgh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3pkumjqhd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dawhfmbx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nnfxuhkb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ickamnkk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3arzspcyq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3cusfpuqq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3hrtqteqg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rtkgqfcv.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3prgezfwd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nxsobasc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ghyhoglm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfeccecb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zpjoxlfh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3sxfgkmsj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3btjkrits.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3srswoopp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3rubcltff.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3frnmfngg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gqzzwmox.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3vwqsywcf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhctphlm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3knbvdrvh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tyrsmatf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qedlcgtp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tggcndcd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ocztfify.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kqzrcdjr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3blarkywe.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jltnbkef.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3igdcgiip.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hllqdktl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rhtppyhs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fhwjdngb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ozoseofa.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dmsnyrjw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ivtxrpqu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3dudxzijo.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytxpadbi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hbbuvvdf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3sjvdzpaf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jmviorgy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3omxrbztn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3beweeqzq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3euckntmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcteawtg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ebfqavwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhxpxyil.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cebqbdpe.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fxklgoiz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uybjebdl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qtcsfsnw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdjiimms.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzgvbkog.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nomlmbal.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3lnfnmmcp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yhhfutwv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dehyaliz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ekrnohdm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jkvxsiyo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbvzrzrf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjolirqw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kvcwjymo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rtylpugh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3espkvlhu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mhzhwhuu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mcgzysoi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3vsjundcm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3njylzyva.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uhorqdsu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xzkbaerz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cizsdogl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gfohaboc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3syqkzisc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3idltbeec.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3uyvuyntz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rlsnbwgq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wszghbwy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bqxfkrke.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nxlmvoax.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nohxflip.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3pukgqvuh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yugzjxik.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kjcwcwoz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3wqcqcyzg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lykbhbpc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3wwkkxmcz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3szlaumjr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bnoebhoy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ddtoasei.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ugoagfsa.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zhkcwpra.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3pmwkkrjw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3arjbgebo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wkemqbhn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3syjgarju.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eervjqfk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nyiiexlx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iaaadnzc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nvngomnj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lzyizrdo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3goonqtpt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3druwrihn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rgkxycyo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ytfbubui.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3xfhhubfk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zeiiteng.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dthcwrrw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pcgzpikv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3uyzelcwt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tegivmpk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hutxhueo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3vrmvdqla.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3sdytgzmp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eofqgvwm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rjglegub.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3mmhdcczp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3asugcnci.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3phcgzrik.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3edelqkwn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wnmvyvlp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3anpgkdma.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3scqbrtpg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3awmadezq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bhahwyus.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdsrqvay.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kacsvhhu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3npqclqjr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wlzrnplc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bacqsbck.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jzriovvr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wkgvjrzd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3zkvarmws.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qyipthav.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3llfpmuty.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gzwyummg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fmnkxuwb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bhsfytbu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vlqukpwb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rqgnggbf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zrtjovha.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ufxellji.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3epozgwsd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xrtmvxsd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rgfsotem.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3renxcczm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fhtpthsu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jyncreth.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3thyytlsv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3uqkfbxhp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3psvrugbn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nufroppq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ejqdwlsz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3upvhhdzw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3suclhjlk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kzccvcmf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rymnwqhy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ufmkbyfj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3koiqyatz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3mxpysuzz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3crqmorgd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajmuqqoo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kozlyijr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wvegmznn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xdpyzqym.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3zprznrrs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3aqzywoqs.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vuftdnwu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fxwriuow.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkceirkj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3hmwqqcyc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3wdniehrt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fstualtr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3veyoikmu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gcyjtngw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3enotvnhg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ifeadgbc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxmkxcpo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bhtpepxf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ybpaulxp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ogczihhq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qugnntch.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wgijvogo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3kjqpisod.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fqshmqij.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3oyuqtikd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3daadqbke.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dhodmzti.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3iwevzsxg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xgxmoqgn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3cvzvpcfe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iemoyigl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hrtpoqcs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3axgmqikb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwxsonew.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sgrazibo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cycrcwyj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dvojcmfn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wunncqzm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3cdrdnwle.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wpuzcqsg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gkoqulgx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rjzdmgfd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dvbdazcp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rjlzehvs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zsyqowaq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3sbblmylw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zlnazleh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zdaksxgi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zxlbpscz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qvrsxigp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lbkpohhf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vuzluarl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dpsxiaxj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gekiaimm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3csmpyubq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3wlvdfnif.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pskazohk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yujytabx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wlqhrvsp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3aaxvggos.html


<!-- 参考信息 -->