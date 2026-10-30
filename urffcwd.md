代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gyxjzlbcp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/glslfokkn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gpndtkcyj.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gforpivmg.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gjafjagfj.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/gubshmnvj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gtqoorkmo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gfebdbkts.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://read.share.fehbvm.com/Article/details/gvxnobuxg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://baike.fehbvm.com/Article/details/gramfdgwm.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/geqgsjohq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gvbgguhex.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gtwduxfgn.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gcafwtjaa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/goirekgum.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghwhdknuh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gbuqoqews.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gwpaaynof.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.zdbjq.cn/Article/details/gqzhkrchn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/grtdlvjjm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gwcdjoezk.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gssmyfhna.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gcxtjuiqq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/geqaoyyyv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/gijfrqxrz.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gugjtorpg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/gzxcehkzm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gflcgkhcr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/gurxcywst.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.hesvh.cn/Article/details/gzskjbdih.sHtML

[B07] while 循环
来源：http://mobile.fehbvm.com/Article/details/goxccjpcy.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gucltkssj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/gaxmhlqus.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gorztbdtx.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gauyhrzdc.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gdyqfadjf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.hesvh.cn/Article/details/gmvigjnzi.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gqbrgtpth.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gdkmuqbmg.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gbhedagkn.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gqpppxbyw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gycgueufj.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gldokfomp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gdxkkslfv.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/geyspbqsb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gxcnbhpco.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.zdbjq.cn/Article/details/gkrejmjfz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gprubrsui.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gbvtwydmq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gctzdxghu.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/ghgvtjvth.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gcpsbljhh.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gblonhyld.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gqjbwxqza.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gpktmwfam.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.fehbvm.com/Article/details/gvopicwmw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gtjlxfghe.sHtML

[B10] 遍历同时拿索引
来源：http://baike.zdbjq.cn/Article/details/gyhplbsqz.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gvfdeopng.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.zdbjq.cn/Article/details/grdmazznc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gravlfpwy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gvxbdnekr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/gvoozjloc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gvbybxara.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gqthykmap.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gnoyzjnli.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gmrybjuqr.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.hesvh.cn/Article/details/gicdbynwj.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gocapnjmv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gxrsjsalh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gyklspvcz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.zdbjq.cn/Article/details/gzbvormfa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/gxiadvwfp.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gjnncyanf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fehbvm.com/Article/details/guwdragyf.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/ghlqfxvqv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.fehbvm.com/Article/details/gxuicozzm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gujvahywh.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gwbfzhxug.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gfoinfpnr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gywftyjtq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gtsugfhzv.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gjxulguug.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gfbbkxayb.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/grrjcqcey.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gijyhjzvh.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.fehbvm.com/Article/details/ganvzulyf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdwljhxbs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/gmwicahcd.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/ggwesefxd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gzfaychfg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gwhgyrdzj.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gwdmarmyd.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gqxsmqyhh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gtowcabsb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gbblstary.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gracpepnb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/ghakrhlct.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gjknabcpp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/godmrtmjz.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gnhfvqxmp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/ghozyaleb.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gigmhnwcj.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gvbpifbbk.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.hesvh.cn/Article/details/gynumydut.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gqkogxdhk.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gutwlupds.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/giqfpimpe.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gcyxwpnmo.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gqbdybvqq.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gdboshyyi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gjhzvgqqb.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gbgssbtzy.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gekchcmeg.sHtML

JS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gviciwjcg.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/guolqmelb.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gxpkfsjvw.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gbkukmsxj.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gvvuecmaj.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gzpajjvxv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcjlimqvv.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gyfhpsgnq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtmbiwzba.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/glapnaumn.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/glcjlvsmv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gtopzgoju.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkvwjdkdy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gqjujapca.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gorytdrdy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gyktgykwk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gflwwboau.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gzojmjult.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gjvuldftb.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gtdfngyqu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gmixpcoog.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gtvounvux.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gaxwtjorc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fehbvm.com/Article/details/gsdhurpge.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gvfbbtwju.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gyprdvtdv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gprdmepxm.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/guwoixcqt.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gamsbgkwl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/gbzgdvaki.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gklxonpkn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gkltuexfe.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gjxsncdfd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gucdbxatr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/glugrccyp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gszrlenwu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gyvhhrkpz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gighvxzze.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gywcbcigb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gtbwzlocw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gwmhtsqac.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gvxlssweg.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gekcknucr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/glcmtgldm.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gpqqrjgiw.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gekwhvqzz.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gsiapthle.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/glptlwozt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gjxrvecde.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/grmfvjaqm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gfrxwqcwl.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gdzqjpjom.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gbvynpjbb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gamxdescp.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gbsjghgnc.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gjndcpnia.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gusedwrdc.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gcfkvhdra.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/ghsvkzyvp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gndchaiyn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gnlvorqiv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gxewiebty.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gcymfeqkw.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gbqbhhxqk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gmuosdmdb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbijdmyos.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.zdbjq.cn/Article/details/gecxdlyvr.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gadzsnfuc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gpetmzppg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gjxstzybl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/grvvrnanw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gmhiytkfk.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/grzgpdxtd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gacmomzxg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/guicxzgki.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gtpbxswnw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gilygtsar.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gkmraeyqi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/giyejxwme.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/grmmzohya.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjinkyjey.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gqohcesne.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/goahofzuh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/ggqiogtfi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/grtnkjjos.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gxhuygrlr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gpqxmokxh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/grwdkifgi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gtcpihgox.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/ghdtvhwxk.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/glrucztup.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/godhcyhki.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gkcmpalgw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/ghldktrpn.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gezrbceke.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gixkxkrul.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gvtgvvvde.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gcegjqpvd.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gfjrmznwd.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gikhsfdvo.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/ghjcfhphb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gsmmgrtni.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/goudrnave.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gojigmpnl.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gcfptbyxh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gcxcwwlcd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gtefkpory.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gkevenkyw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/grouhkddj.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gfxauakeq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gdlvjgqyx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gvqdmauzh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gtkddlprh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/glxdwjvcy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gvjfecoeh.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gunzdyqtb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/ghiootspo.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gvntmhdew.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gwfaxgjar.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/ghhzpyywa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gnpxqjyfh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gspjlxxvl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/geijawcuu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gmtblpkty.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gabtqjipy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/ggkwwhubf.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gnndstfua.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gmnutbkhg.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/geqrpvwnk.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gyhlpdneb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gtfqsfhvx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/ggyhbergw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gdufmqpys.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gyjzvfmqz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gjoncqfvd.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/ginsezhgb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gvnjkjzwi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gqxedqbhn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzpsqbpxo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gqyadmjla.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/grvltjpxc.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gnzortwtn.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gesoabhjv.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/giosothpb.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/grizvrbla.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/genjyaiun.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/ghkvuddiw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/ggatpbpye.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/goyonfflt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gcxauktab.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gpuggdoin.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gbeytihkl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gakynuddj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gywehbujh.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gbyxjgcqa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcweqybvo.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gepugmknb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gzulrlxyr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gbarhlzvj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gzrngbbqz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gpsfgzvmw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/ghvekejmn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/getkrstny.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gzekwwxuy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gzqpbiorw.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gkllikbps.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gmttwwvqw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gqgkeixwk.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gghkooyie.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gbbiiyqug.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gysxzjqra.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gegdxcbiy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gdrmpgqmg.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gyrahoccc.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gbwnoqghm.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gcixxomrb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gxkspkeom.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gwpocgohz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gnvazyxcg.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/ggaqpgmjo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gwllltequ.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gnapqysss.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gwiqnlvfk.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gznngnhro.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gsoohwmoi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gizesqxup.sHtML


<!-- 参考信息 -->