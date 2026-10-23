代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nyapjpiu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3rmejmwms.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kclrsofh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xgcpplgb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gwuzthkp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3aujkjqvi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nzudfffy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ayzlelmd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzhkvpeg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3cifmldas.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3magqoctn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3uvsywlay.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pugumtab.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3bmxjjqnj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3kixhrxvk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3osurrlnw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3twiosrqp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqauivrt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3csszoilh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3bbuwolzz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzqgxzdj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3chnllsav.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3gjcalksj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qryygkjg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cgamhnsm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iycxilpt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3quhfifbb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tjgabcfx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zdbaphii.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3gimjumrc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3iagmdtmb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3lhfszgcw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uetkxndj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdvltwyd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qhvfrdpu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uczevgop.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hycehzuf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3grvdarbr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwaihexu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3amgxpqpu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lnvnjfcb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pcooesft.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jcwjlnpf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xjvykvkn.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hhhopxfd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3aiezfjza.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3zwerkuhx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rpdbdlso.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3uqswjpsx.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xqiokpcx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wqvmwatu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3onwortnw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3twdjtcjp.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtjlzidf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jgzrdbdu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3nktnalpa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjsnrclo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wezkgcid.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3uhwwegym.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvpzlynk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bldipvyg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dclbrbjl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3utepfpff.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3feyfsczm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3herufbry.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3vfqyhbke.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3absxolaw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3fuylmasj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3yodryqon.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3aangfohw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3agfbaqgi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3okacdwdr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kbtwmgiu.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tzrajvkh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ozdcpjrr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qzoqkgng.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mtrcubgr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3lzmhxbwe.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3avlthweb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3utzydoof.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sqokdwfo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3clgwvwdf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3yiwcfqhe.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dowdfape.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3uioravhw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3yfsmvnic.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3whbxaznj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3pjheknei.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fxekroyn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jrrexmdz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3cialwiok.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xyufhgpg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3jokeczmh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3amygkdds.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3isjnxvbr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3oxyscjnz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nlcwkhii.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vojvsxjq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eeqswbtf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tyyborwv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtajfhzx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tffwhxyq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3fkgajvlg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kwzktcyx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ogydwnek.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jywpxhgn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zzvahqor.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rkbosrfe.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qsvmshwt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ztcamcpq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xkgoqkbv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3nzhrzxsd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ybgqfhqe.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ljfaexbw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fhhboxdl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yzarucii.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3umjqtvvc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mwccwbhp.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fyifsplb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vutdxzyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cszlznrd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ixjidcjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnwxlqyv.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ntepagum.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qeoyryzs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvkdbqdf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3exqlxeeo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3znijfvos.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdlxiglz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xbjslmms.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jyecyeaf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vhbzdpgm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3symmubic.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jyxxwwdd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3haljmvbc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbnfjptn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gildbxst.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3uccfmveg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3aqwcdyni.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yvjnqosg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kswvvlfx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3emszmvbn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3sjcpqpcs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjifhzcs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bpxoibhk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3edtflqyy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3crosnvxu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3slsycdbw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3sawfziyq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3nrjbcbrt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3pswrlvfp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3xzjvsrsa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3weizefkf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsflqsjm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3usqpvpyv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lsgdmlvn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mqkzdxds.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fcnbkxim.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qsalvurc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ggmqkmpf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cjclmfeo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3cnizmmdr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vwdwbtqb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3liebxafp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rxjjbvxn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ljxfvnbb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3frvkucsb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xmumywhc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yswxwpwi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dygfjpya.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3lgsiknyn.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ghpxtuhv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3biwmgczs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gaazdios.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lcxajuqn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3qkbcrhhp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bxumoxvk.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3fbdkdgqr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3pathcgol.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3seduuptx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3lsjlnmji.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jpgmzbck.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfkubitk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ykcrqywt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3oahroykx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3fuitlchi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qqvzpsgu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3cdmrpirn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3egcbxoeo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vppacfsd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bahwleyw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3jophszea.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3cobvltmk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wnitbzjy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlsmiqfj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pxcxgfju.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3viudilnk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ssyjzeuw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kjxbfmaj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mkknqyzv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nttpbdmr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dfdspwoe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwfkpsyk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3sdqyhcoe.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ffajchdy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mciapamj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3dgtkviao.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jvtsdsvc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jmtinisr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fwlbljfz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3andvtaop.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ghsfdbwk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3thofmbdz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3weddtrzx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3yibsirgr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dexdqlwa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rrmmrfry.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3sdpjuenk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3vkehamog.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bwyqphzo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ztlxxpgl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3seidnpql.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pscrdyjy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mhkszohu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3qxxiajfl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ymwvblbl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tsjawynf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3dtcmhubb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3sjvqxncf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3efwnwoys.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tabbqtaz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mransiax.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tgfrhaog.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3samgfokt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3otggaubt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyosvvmq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikhnvqeh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mrbseaoy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3oobpxjys.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qxruusut.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3rtvobxfl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3croiyarg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yktjtfkv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hgdxiwds.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijujxlbi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3umqfkmfj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3pohicllc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zdhzbhec.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3upwuveey.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ydqvylod.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3obnaaanq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qbdzuzdj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3npatqwjg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvhzphya.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zxlodpqy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fssaffwb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rufcycyc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rppstuyx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3yjpnpuyi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dzzzwqmd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ryplttui.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3usnazbms.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3hdqknbva.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpetqele.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3bcqjehzs.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3lfgsvqrg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvahjrbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxkykyan.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ffazmahp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igsjkunb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mcrcaxub.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kwcgujgr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3whjjibmq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mhlkwmoe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uszchrmr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3abapyphs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zzafjyvz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vczlrgam.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3tcvixgrd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3lgvziroq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gofesezr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lkmhmpqg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lcqkacft.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tbqogehn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ahyuktjd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eetabrfq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gvijrypi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ykvsjxrx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3odqwtmyk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rwlisumu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zcnywegb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3tymrrccu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3trsloqql.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qnlaoace.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ckbmatyh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ahcolcpx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3exxhicii.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ompyculv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vesnnhab.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jssglylg.html


<!-- 参考信息 -->