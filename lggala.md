代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2utdvexqj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2kwbgucyr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yarqlokm.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2urfbsrru.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ydsdevqz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvcarksk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xrggnbcl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xnqqaqtf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mlocwzui.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2thfmlywh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2sokshggh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwenlfxh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nysanazb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tlakwizq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2msdpvbxw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ojtxjfvs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lnacilyg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2unnayirq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qazenrkj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2frwegmnc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulssrydl.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wfbknwet.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dpyiqqaf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmirgkxp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fojkhjpb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pjenshcq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2kwwogmfw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2trckmcay.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gplcboxy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfwvnyms.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2haonoiuw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2gblscuzl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yctcybfl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bixwxasn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2sikwygji.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nqpthlig.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2eirzxujl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2xnloyjhq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fatqacmc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2oojsuzjp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vqetceao.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dyhlmdmy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lcrqbqar.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zfzhfpbm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2onecznme.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rnrakrxm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2tprtpfgl.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xbjvdkzz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2sxgyoufl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2pfuacxnb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqfoneqc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpphrwbf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxxagwhy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2smpjsind.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2yupsfurp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2eqzuauhr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2defouadj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zfkzacar.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2kjxwgyyq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lmmkxdnb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lsbfdrzv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2izdqaspu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvssoamd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kjjiqpfh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2tpexzqta.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2glruivly.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2aneheskp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ktyyugid.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2nnppwygg.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mujzvqph.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pxvmxdhu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pfrbguja.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2teyogvnl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2vcxiawzn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kfugiuje.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ywadcrzh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2vwqknygv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2xtutxtqr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pbitjpoy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sibyunbg.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2imvxosae.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2bmcirubg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2uecrzncg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xgqifwas.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2mzwzzwue.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ewgzqnyi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlgxnpsn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yspsqpzu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fcymmubx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cuojqmlp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tkngngwe.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2aufsanxs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2pqobnibw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2nhkpxsul.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2adismwvu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ngjytgyy.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2teycdijy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzgjirem.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jctsdykw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgpxguvm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghhgnrby.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wpqvfezx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zkouadkk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rvntdxlq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rivwqatq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pxpjlomb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jsguytlm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qonovnaq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gdlelwnj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wdsjpvog.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fjkyhhbn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wqkcxhss.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2woggeada.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zstmprek.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ziwapoyf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fmbuldcq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kdfrfbqq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2bvmbsteh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ybcyiwhs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xglgqsdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvbiakvc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ozjvtlxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anskzeqw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjoladwe.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2emqmntel.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czxppnxy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yjxkqyyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfigtfvj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zepifimx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ageokezn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2nhjsfadq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2puapwtrv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2brftegjj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fznmnvly.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgmryfwf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hhrnbtfd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dmxtejof.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hyptstmv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2yuhryogw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2nlukxgkr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gbvjdjwt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2kqazxfho.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2xyjdbqrn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2btbjbvho.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ehlomuzk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ygrbtpca.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2jmtbebmw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2sjlsgzei.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2byvoldjj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xvlgagdv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2lqkpuuoi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mzzzihck.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftftcaho.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2spjhmdni.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ajiwkwud.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2bdfqclwj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pnbwuwpt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rdhuziuc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyjhsuzf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jmngcblq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lyzydhuv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fdsnhjbx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2swupqwzz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rudxsjoc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2janrqzux.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mlajxyfj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2habfkuro.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2eeqozzuo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2yyputeqh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ieomjqjl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2inkvywgr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yzgjqogl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mlygqyqv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lelgkbql.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2zcqzprym.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fclbrwcp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rzwabyxe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2nczshguv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nuixliho.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzyutawl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2cyzsckqe.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kgahyctf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cftdqbfd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xlszrqsg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hgrvvyro.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kdefbady.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wpetvvoe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vxkbesyx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziiacgrn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcfrlpso.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rvsnwodh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2iiftyvkf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2whrptdfb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fgtepiyi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nifyfxeb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2voerybrf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvknvfhc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzgwfawh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yztkfpkv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mmoqyocz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtekcxdr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mgrohruc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hfdktnrh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oxzypaqr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2juarctis.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rqlhesqo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tzqzgztl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bosibwna.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wjtlkmzr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qagrclvb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bnklwtfc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2emwzjjzc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2emauvjtz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qhzkbvle.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2azmhbjnd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hzqalsep.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wcnflror.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2olokwdgq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rgopoyoa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2htoccanb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wipjgshz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2tlejdjlw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2auepnbsv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2speewcso.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2bugnfbev.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vdxshhrc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2aorglqyu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ynpxkerp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ddcpthtf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2uxxnthou.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ypaylvxj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mgydupjk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jjnbonfk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlgphpoc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2idrgwbex.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iqeffyrl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hmsvxpvx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mdpbcsll.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bynqacvv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2duetphqt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ilzmwdiq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mhajtkwr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2smzmqlqv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aagfeqln.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hhogacjl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bvbaovzn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2gcpurofq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tlzobmvs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fwbulrib.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qnvimnfm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2juwpuwgc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wuocnxdr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wggssiqn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2cshursxl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ukexuump.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hgglwmsl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ivgdikgm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vsjldatj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hifbgpbh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ndlgaeyb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2riqnrkjk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2atdsokdg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2qygqjfey.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qeqwihbe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ydsbmmru.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qjnvoxny.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iocmbdjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjcosykq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2czmujvra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzurogva.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nacxglgw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qavojfia.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2grpuljed.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2penzfcsu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fzxndszu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nnrmmbwc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2cahajkjb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tbrsomgc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ollkpfsk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nxawrmes.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mxbdybvk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2dkassdmj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2juznndqt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tovztjst.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hglebrkx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hupbwrlo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ndjbvyeo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2klsqqofy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2oyhpnfpi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lglnvenh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mpukuzoi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gewfqcwf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2croimkfz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wnkwmwow.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wjgzirbn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2zzgjqmrp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bbejbtak.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2nttizmmy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2vgmedomc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zasxhhjw.html


<!-- 参考信息 -->