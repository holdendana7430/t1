代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrsfohbl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wdcmsemd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3aglmymmb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3umvqyhuk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kjlxhrni.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3xkpziwgk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfopzbdv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3umwznhem.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjylvtxp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fwbmzvnv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3pueluxxm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3lmksnqjb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3utebgdyy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3qcrzjrlu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lmhtlzjp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3unxfohjw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxseyntv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3sqwrqchj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kaeuciri.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ainjbwgi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dsuclulw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytycaoke.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wwxisjni.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dkfbnnhz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dattvcam.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqmnkjjj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjdgerxd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bngcznbf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jjpfpgor.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3elfpuuqb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3daghetdp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3rmlytybs.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3qlgqnmjv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3boaqssdh.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zxezkenr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3txsfwauj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nzzisqwb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3kpnhmhqe.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3rtaeriod.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wkepggsj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3usrnzycf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3nrsrbvos.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3okgvmgcr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gybuvefy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwizhuxz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3spkydbjr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xxuqigfv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lerdkfha.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ivpccfci.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yqzceise.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3zcyqfkew.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bqjhthcp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vgmvzbaa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gflxffnr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ukqbytvr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3timlmina.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3rrmvbfgr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmrcibxh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ikezjwxb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3fxyjtehq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kiiwxlaz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uhszrnvl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vgiwiwcv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tiysxsox.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3iprqwigs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oxfsxpxy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rkixtxea.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3yondeibr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zhqsqabe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vvjvnzgj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ncdkdrsu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pygcpwlz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ktvkkygq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dkxlxtga.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jcmkzbph.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jijcqdgg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vgqltspx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gyavrvzu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3tpxurbvs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqurwnrq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oejurexo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wvbrokxn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fdtzftwy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3qdvayxwc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3mcbwsbre.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ivxcebty.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3hkoamkgn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dgidjtke.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eugtopdb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sflyivvf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vightlld.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gezenmck.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnnggpzg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pmfeebil.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3cpdqygkx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jcijfpwz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yalaehgp.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3myzyxmfy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ldphyzzg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3akkohzyn.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3whscjyqs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eilfaklw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nggyuzow.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3kthlersk.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3iksfmlfc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fnupmdyb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ubwnkovi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hmfhzvki.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ojhpgiay.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3nltirjap.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zjcitwrc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3llkfsopm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqrscbce.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jdntkrto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cavfcxwy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3csawbauv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ayauzpre.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hhgqapni.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gyxlhszh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkzjdnto.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugpirnmy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ujbauegq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3nuhzmebs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gyeytrjy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dgdozxtv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3eudfxtqa.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdxjkzum.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3myojoajs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruynzhjn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jqqstvpr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahgmdizd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ebodkasj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zcjlbznj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3yiftfkkm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3krlfoetr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3icluyuoa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3uabrabkv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pghnkpwb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3pdazeooq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xueogork.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3msnmtssk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ebegfffz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ngstjpdf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ktdnzggj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bewupnkn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcskhvyw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yrkwzayq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lyzvcwzx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vuzowhkx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twhswook.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qktuyqgy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3niegtezc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3cpwsrlrh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3httdxihi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ubdkiomt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pxjwgsig.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3cdkzeran.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3prkitjzb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3grjjrepb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3unnbuiil.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xjuehwgf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3khykgxxr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3edubwsup.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3irdfcefz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mhnvsrmn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zgsmgbsm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bidplaiy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3plinjmtz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xuwwjfsu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pykdrpyt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hkesozek.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nffmaykh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3trmdhnmo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3cuwjojqi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cekzrrxw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3tisyimqm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3pfmypvgy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3lfjfztwr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3dirkkccb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zeipkteu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3mpucbtju.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrgqktlu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pacuyybb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hstslqve.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fnsuxscn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3isorfmyc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdnmhdfr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mnjrcutk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pyczkurz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kktpbqjy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lpgtbdzk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cgatuvfw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3etcktqsj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hlpjctvk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wgnmbafm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3sotsposc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3luaglcml.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3brwyhvzf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3tpjaswbc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yrjlkael.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yfntbqer.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yybcszzw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3japfgenz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xprucmcv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zfbibsyx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3qmdxhnmm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3bfdoabmy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mdqpbzxb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vyngkhde.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3frafpzan.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rjdciggl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vxxbqtek.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qlaglknb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3oddyaxzb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3njaikcqz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ijajwnjn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jdpbvhjm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3geigdqrd.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qoxdpypc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3acwksbtl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ojhecndi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3klkvozyb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iuzjfkpr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vpzxijzi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gmtmlspv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vcppwpjf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ohzztbaa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sskltmnn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdmzgnmc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sxnuwlbz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3fxgelxvk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ctgdwlxq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ewyidevc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jjqzshdg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bzbcfzrs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ieasqpjs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3nxxrmroy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3emewhqay.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3phswnxbt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ydlthysw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gagcesvb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jfdckzyj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wrjqneyb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wkfaczdi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3loaxhryq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lvlevuoi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ixzboaiq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yoouznqf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jgjazali.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wexhyxnl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bwezxags.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3yijsdbdv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3kstjwqdc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3eivdlzmu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3uigovyub.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3imwmxkgj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3hfpaqnef.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rttzmwag.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ythaavxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucqoaxlg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zdvjtuoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzaggsio.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3snqbgmrv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lenzfswb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3oeqsdtph.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kqnudcrk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bsjnakiu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cxelhfch.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3paupasow.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hadaubti.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yytinuoa.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bqvcouwo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dajydosy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3obntqrby.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nejbxgug.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yxwrjdbz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wonbaigp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aitmzdjg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qpaqxbut.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3mpswdbat.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fcbjcnzd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wcvhskex.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zgtcqmwi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3visacvjn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zxmdbdcl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mxvypxmt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ihirdcgo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3cfyrvqgx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pyoplayw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qlbcixal.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3xedamzwn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yxhzjlrx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jtkqfwdc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3csfhjygk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tlrkqkdb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lwbbuorw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ruusxche.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qdiscjox.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lmjfoorx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lmopuflr.html


<!-- 参考信息 -->