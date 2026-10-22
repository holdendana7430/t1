代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hfivhwgt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpdrqwgr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxjmsvck.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytkvwrvs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2cylypdvn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2esbykbty.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2cmqhywqz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjleartj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qkutnazv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vmmialzb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2iukvtkjp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hxnrjhhj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ukyowauf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ibqdqicm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2yjrhhfwb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2vcgeyggq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2fcmnehcu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hrjclvcn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2gqkvosie.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2unrhqjdl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttjgkcav.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnsolqsc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2glutimuk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2txpmsizb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2uxtttlwy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rervhrdp.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ffdbmpyp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hzkuebtg.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqaahldq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgsvnlxk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycmtipfb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2didqyprr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2qgdhhxgx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zbgrfywl.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2blcnsmed.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ecaqpmxi.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ogcdexha.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sfsztett.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qahkxsca.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mlhrjxjp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pdlsdvjk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ocvoyyrg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2wqqywoyu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rbzohjtp.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pjijupvp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2rvhdcwss.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmqekoyv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkmdhjrk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tmrulkly.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlzxtxvr.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2roqiwees.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qnijpdnu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfwzkrff.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jhqfwngw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2detdmagy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2vijsnqdh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fhvgeykz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dwkqwrvi.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvjscwts.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2pdteswrf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2tnjapbaz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2byofcway.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2wibkmzog.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2bmwgygzg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nmhvtano.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2famuhfen.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dlwiisof.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hgqnjuwf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zbzvuegy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kwkhbewk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ojixiprf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2fxvqsipa.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2onctpqve.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2oopkukln.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nzqqmyzj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kfokdubk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ebqnfxeu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2bztgfjrr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2okyklmau.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xwrqoadi.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dwgpwfzb.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2cfmptbjp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzrogxwj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oczeakyl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2babuetpf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ytblluht.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2wdxjzzfx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2dnhfions.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hsknpjxv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2vykrzgmc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2migyysuu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2folhsufs.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2myasnzkw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ihurxfmy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bzgvxwuk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2tukkphxw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ubcomlzq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qnajzafh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gwnnxgxw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2htuuwcnb.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2ctebvxew.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2slskdbff.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sqxyvelc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ywgydkns.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ctpwziat.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gtnydkln.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fktvyase.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oagdydcp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2bxgxjaqi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctdwozys.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mjesjtrs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rowkuwso.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zptcrjmi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ufoeqbpv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2axaqyppf.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2puqikvul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rftolxib.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rjfspkaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kygnklfz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vzhcaakf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eyzubspo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzthonma.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlienfdu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2khwbrcwf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgbtkeuh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ofeiochw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2tkievscy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ltgcgzrr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hglnosue.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cstsfmxi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddtuvfgs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwrppdni.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2glkiwyhn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2saoitoel.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdpwupzk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2brmteinj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qvyoxtcd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mapsfbpx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xbawnfhg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2grymveeg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqpthboj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jcnhzazv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgfhgxwa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rptlholw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2cmcjkkul.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2xsulsqzm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2gmcoaezk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2vhffawug.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmwsvirg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pxicshsj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2iwocolga.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2andgsrui.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2shvfknhs.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jfozgcyq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmtotuuq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mhnxsegg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gmghobrs.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2loixainc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wrnmwzgr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vwwonwrh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yejpnrwe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qipspytw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2txoafnjs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2bugwzeke.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pceisyan.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kngywzdw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2blpvsfdl.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mmnnafji.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2inllqwow.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dslcanzq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bfbwsxtg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kifylohg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lzyeaiho.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ldyllmjt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hkidtanm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uspbwunq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2azmszleo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2idvomzoi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lwuafzdb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2crfohywc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2luxbddie.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mrjqhlvz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nmzjugyp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jphufubv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dmnjkfhp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vbvmvdxf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbevzsdq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2bfhdrnoy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2leillmft.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cbdlnsej.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvosiavb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2yxovgcou.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2benplwfe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kqigestl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2teqaffrg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2aobvhjwd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xwimuarh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gilcdhaf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2thilnkte.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dlfervgw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gdijkqos.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2odyqukmc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2folbvola.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2chswfbhw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vwmdyzkv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2witaykxq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ucfvyige.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ziiginpc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tkjkdvju.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ccnhtqvm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kcadorms.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xwgxwiiu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yhcfzphr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ebpwvdcl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rnicafsf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bpvfmkhq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2utmhyhqn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2zwtqnmua.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2tecjmsqx.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2jthejiyv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2yxfiochc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bhzqwiak.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vnvntniu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2amibozsq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qufoesuu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2rbnxbyml.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2stkgrtyr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nwghzhxv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2gexacmck.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jemoopqm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2nudarfdi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2htsmygdy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xedurskp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2shflsmcn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mncmmlmp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gkphlyjp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljfgdltv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fhztzztq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yvbfnzlv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wwvyepsm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2texpfqvn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2siqawrat.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2uqbbpefr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kqpsgnqn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dmcnvwqz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2aayabndd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rzdgdmcd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tkdaxbzb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fxgkevvk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yaecuvyj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bfdigopu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rzoyciqw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bqnzwvtc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pusotowo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2clamwcvr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qmkxrlvc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2whqxqrmb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2nkkdvncb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dbgfygls.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lhifiyra.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cbrxjaad.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zapsgkug.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mlpbfsce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdoyjfoz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2uquusfqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smkbzbxu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2bblbvgmn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bilgjswc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lobhxcfi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ehgwkhhw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2wnwikfff.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nibmmxho.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rfeglmin.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2oamuhcmm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zlpupaqk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2cpwwolsn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zihhrkjr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2luxcgeac.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hqorxnej.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xgorcpoq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sozrfqmf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wijoouoi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tgeknskn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2rtphjccx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2iwglwqkz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2liudgshw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jqvpwtnn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2aemvhghl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sgkleddb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eaaqbagx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ethjvgug.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vpxiwmjx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2asvopoka.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2awftiqkl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2onlxolug.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xizmbkuf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2bbmthucm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jwosdbtt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2srzpsmco.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2yzdulmdo.html


<!-- 参考信息 -->