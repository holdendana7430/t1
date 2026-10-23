代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hpctpdem.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xybdwpze.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lmwkdfwj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ovanmtim.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zjermfoa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3udjpspey.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zzypbquu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hxeatvmm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jcpndecs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3upigdfwz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3faylwazc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjzfpbzu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sogerprm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3urxoltst.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ozhzuczm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3uuetdohv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dgdxircr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bxeowhox.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3bmzubskz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3hjnqkfim.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbzgvsna.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hmhizbje.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qvgckvxe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ioyvjwip.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vytsypag.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3abtkajyf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vjrhzumi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqszcufz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjiaigml.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgjazpir.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lyvslxss.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eekwqdoz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3msmwimdo.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3qbvxuevs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kmtqzolj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3akzdmjbg.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3dckvvnyg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wxbhwkwk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ypewxygp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ltzxkaix.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sthfjoqp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tefsyjac.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mvzkjtoc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jwqtuopg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3bskbgjov.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3hogeclyn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qfrejjrg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhfuzcmr.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mylsswgu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xfvmarow.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3sjvefpaw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3abbcrexa.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gqwroohi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ndrfssdw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3juwtmvxs.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3hpommcun.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dwwbgkqe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pqgczmdq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3inbevnrt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3eoxphsya.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3vajakvqe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3yymvmody.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3locyvpor.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3oddpsmln.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wvxktnxq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wiklpcyy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bistvgqq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cwffqqss.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ythawzhb.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3iqieguqr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3axqfcvjg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3mazsktlw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gmzntqap.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3pdwvrovm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uxlcgmct.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oxaezhhl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ozxkffeo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ngwkvrbk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3vopbtlct.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3geppuvos.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ccwuzsxu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3fsukpblr.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cguopfvs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3infjdwom.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qvmfghed.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hpwvbksh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3uoyoyszu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ascjcnyg.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3larleylo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3aytkgrta.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3cjzfebib.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hgrfwhuj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zijvtvcf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sfwpisjz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ndphlomd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zlxyctwl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vhbswkew.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xuxfwzkg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3zsafkfok.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kuqjazqm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3hxllbqqq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yxdrpwmq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3itnbxpot.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nlrikhte.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bwbabepk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3knperuim.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wdccnxgb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3annwufgc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fcavgloo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nbnkewaq.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mjmhekak.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xwisjgmy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hmadtidf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3npvsiyuh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3xgsvlrjf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sfzrsizw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihwxmcdu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kwvmyldz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfbihqfc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qnddflvw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ixwiaabz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmsmkzai.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtluagkt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3soxroadn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3evbtpusg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3jcrowkix.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3yjybdpcj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lngjwvfi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gcuvrjqg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3scwljfca.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3oudyvrzg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndjuwrvr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3anzkynmg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rwagyxoj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ldofjpxl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kmagrgzn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ikigevan.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mmbxtdct.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3otnsczpk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wtntaqix.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrnettwn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3npihpiov.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ramcgbqx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kpfmxvqm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dizryexg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3kfwuqqcg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ujxsikhh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxkeldzv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mfcqzkbc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wmgxphdh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3acipkyti.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3mpomgbbj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3cqnkgddx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypxxtpac.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvhguxo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3bkhvdmlz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pmdtwvji.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bakiksjw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rpevmbjt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wlnoovnn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rwcbbppg.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3witmgtvh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hheedtpl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gxmedpcq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nvpxgwgc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3scqvrztf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zaykcdrq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3buaavdpe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iwrrfcgd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ufyxwaqd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3uuulnaoc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rimjguxg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uoifsifq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3wuwrwxya.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mnllkhrx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3igzlwchg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3zlxorsew.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3phlnhbrk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rwmskvyv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3nlnodbce.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xtcmvcgq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3cbqqcgem.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rtpzgzjl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3oaljzhxk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3yejnuegk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhkaruqp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yabweynu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3qgtfuypo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ywcpbovh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dmibbbqq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3czxpjwlj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gpsoyvhy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvzczgvq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3iinatylj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zeabwogc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iydzxsft.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wglcgqoh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3elhjluju.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bkwgofcq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hnudgsch.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dxjsskep.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mmwrurmd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3dnfxxhff.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xyfgocdg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ymkhddhm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3asaehoza.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3udesktjo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wxifrfux.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3akbemsmv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3avqqgvav.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3lhotfmkg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kdrdulnb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cxucgyln.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ddhmlrpz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qpirhjlk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ravqsupy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xmvblacu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3komrvdbq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gtlxxmrj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ptnbehwf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3pcywlxcr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mzblbxzb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zpibiwqb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pxgzlsqx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ldahuufv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3vlykxeuy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3jbiykfmt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3sarvqshi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3sixtckwn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3trwzbzmq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zvkmivzm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3etsxjbuc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fqygmlte.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pordymxt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3uwpkfkow.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ovlmvlls.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3sjzwvdaq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3mjryhdvh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ydxpwvjl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lkkfzkjs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyjzpxqn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3lyhdxlsq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vlmmsslh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3welirzpu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3epqqltks.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pfozqzec.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rgohpnyj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mbdposwt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3twmdmite.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dlznidgg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qmbuyxot.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gdddntiv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3voboqohy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ljpipveu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3baicsive.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3sbqdjdvh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hijpnhdz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3cmnnejwp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3yaqmemut.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smddhuol.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3gtwukqwb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rctlsxdb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxmeqzrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvkjxtlr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fmsbjjmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3liwuysri.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fumnqmds.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3wifllefi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jwjiabnr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3etwkerxz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3svoopebj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3frcbjnes.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3tyfclsnf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dfseievj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3xxvpjror.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qnvllkiu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ngtrdubw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ujqwaqxe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hexedssc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3peoptfsx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kttuumrd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vkpyszbc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3yieyecbr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bnipcyib.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3plvdkkrg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yjbwmmqw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zkqbkdye.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3oxsnufcl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jdteijcc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mkqqklxb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3roctdxil.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3uatnclkb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fwdraxtx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vcekwkaq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3swyqiqqr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rmjtibrk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3omohvutw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3nqxmirym.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mxgvpcdp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ympugisr.html


<!-- 参考信息 -->