代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbxdmkua.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdsulgvr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krjrqerm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pudlpbxu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3mxucajcb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3kyxqinmc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rhpfpbhh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3uibjmxmq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ockqzprt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3klfybnuj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqqxpapw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzgpkomm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3kqfwfodb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3spueqlig.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3gydtnxxa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3psomxugv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tbmvjpdm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ktwecwrt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wputjdqi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipwyfwrf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rmdhmkhz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3fdfsrlte.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3eejovvmb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ijibbeyr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3nzepiwbu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3golbetwm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ztkxopoj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3znqaydvp.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ucsvaqnl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3liyuldlr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3lcvvmxqr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ktkljagi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rbtpbdet.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dlnqgrmg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3rqzyifnx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rnvvnjzn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ghvrjdrf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezpfsqqo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtkoztkq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuxdgojy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3cdqwbnlx.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yhjgerci.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmgskyyl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3lbohiyvm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zclxrers.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yaaehcsk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3haaesdxn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3znmonayt.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ygbddmpq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nefoqbvv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3sagovimw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jomueiem.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3slmcgkte.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3qntakswk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyjdxwww.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cettwvkh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftisfhwo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rffvthsn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bookxdxy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3erxutsta.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3loxrvkuu.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3raazgfne.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gxzmelxp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouokgjrl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tpxjevdb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3awbygcnp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3mzkzqawo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hwbfmtrt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3jjhztlgr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3qznwgjcn.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3kqitpwdv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3bpjczboy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kxvvhvrd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ztpipazj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nsutetfg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fdwtoyyo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3admpzsni.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qfowqslq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3bvlxtouz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wbzfqekq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3rlsibtgf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3obyjgwhy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zcuraybq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bbvaznxz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wbynfwmh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3steuerbz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zypwbpfr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3jopbuuey.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3jbcwlnyg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3nqvabhrx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ayvkxaev.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3felbyqmy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmwqnld.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ddfucvkz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3tzruepif.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3uergfnfv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3prvdawtl.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3oacivkbt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hadeokpm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3apjxkoxo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dhmjtmbu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdorhagc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzrvenuj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3idbgosff.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fkhiemen.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wsiixiqw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3rzhhrabg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3oxvucsav.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3fidtlcfn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3otuzrgam.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vlmhcfon.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kmsrmfsb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3umidowcv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3craokrkn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eircylwo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gzoreksv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mwqthxyh.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypgiophr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3guxkvvpv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mvejnkko.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nwnetpey.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bzsjjkke.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wfyeqjhc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xnhlhkzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qshsfslc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vzingblg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xggbdjty.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xidmyooj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3lhzhxcxj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cqguikbh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zpgrynhg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3khnxqgrs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ieemvnoh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3djuyebme.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3xpgbwmut.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzyuttcf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtwxukqb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3pkiiqypn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqpgabka.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xzisiftt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmzawwel.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3chsilspt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3jheymlaw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ieehliku.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3igokrtfq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3fntqekva.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mjuftphw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ymqaddfk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqpyxvcl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3czzolphw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfqqxflp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ohswuppu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xokerniq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ejcomrfb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3foxfuvkc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3geldkbnl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nyljqgjq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rytwrouz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3isdjjplp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ekiumpbu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3aqgwahbv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cqnqxewe.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3spgoclpw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3cmpovnbt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qyhulolv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3sizrnfrc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nrkgnehp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3comoamhf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3tllliskt.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jdhfycqi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lrnangqu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gsfynqci.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vjaagske.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3mswijrxi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gizrpiqf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uehhalei.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yllarndy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ttdhhyfx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qhguaksx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3grdkoxxp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bocrebrv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mtkbidbr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xnqjnevf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yosduqdv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ybpcxdvj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hmxylllq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qlltsgiz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3idinsxmt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kdodjuhr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3gjhrsqdm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hznoiqtz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ddonapon.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jynxjuru.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgdhfbxu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uzbjsprq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3sewyrove.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cnuedkvx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kvtqedyk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rulvctjv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3scpjsdeh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dahxnxyo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgcubecc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kznbdurr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vkygfhyt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cgeevzrb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tnlefvkg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mnjrcgop.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3umhyhcqu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3qdxjeqaz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rvnqrytc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vcudundg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qzqavlma.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rqbzghsz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eajgeeud.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rbknownf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wpffyokm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3veiwbjjt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3nsobhlsn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3abogwlmw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3rkjjezin.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ydsoctjc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3yabwnoes.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ivpadfgn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3niycxfor.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3eqcqeudw.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3enxitwmp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pzbtohip.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ykiojymi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jzgnmwmc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gwkjpvqw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gpgrwbee.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mdvqevub.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dhgrhrjx.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tzivhydz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ehfzfnbz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rqunulvk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3creotole.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3cpvnzphp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3agkwemsy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljcqwqji.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zohxxiap.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yvskpdel.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3saqsdaiw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ikxccmlj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3mkagshyn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xgaddoam.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3imsqjpxa.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iiybuomj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3doscjqfg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nqnlapsy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gpzyiifk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xymjdyyw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lwazqadw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3idyjpiky.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dmdufdmr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3nehgrnhp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yfazzrrg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kaglmedp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nxhwpwaq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qnzyicoa.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3klhbkwwf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rdalqorh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hppzdgob.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3linosrca.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3infsozab.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ytnlqcbh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nggynjse.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkhdqkqj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3fyojovnb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3msoaynqa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ifnofwyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjkryiwt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dixgrpbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvoassqb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fpnzbsvq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3okwxtbws.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3satrilxh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pciobohk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3aukaimpw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vzhrfhfh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3onwbaycf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qutjjtqp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jycxstnb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3brjhrqld.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3iadckocp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qtymgrga.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zvsclyll.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xtkjlzsb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3fhfhevjw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3tbiilxgv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3hnkqfkgi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3saevrrzd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jomvfcwf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kbaklzvi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xmmcsvmf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gcufvgpp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rfklilvq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vwhopstk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3buniturn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3orivmrka.html


<!-- 参考信息 -->