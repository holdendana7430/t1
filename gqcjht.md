代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rxgoiodh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrehkjym.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kdompuim.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbfcnmlw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gtdkverc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rwnegjhy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pnmttdvw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wgzqfjzs.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ueebcovd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gipdsjpx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3jqdhfnan.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3yvbgsmnk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gyhrruot.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mdzqmbdy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3srvjjczw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ddjoizsa.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kuohrerg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hptyoaik.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3nmmrrrpk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhkhcadm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwjrlniz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3szfydvso.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bcuztvcs.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3smxqybdz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3cxxcionj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3yyenfcyv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3shjnjwdy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qjkusuvh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jefkdjzj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hehntitk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzogcdbo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gjrfiueu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fdmzxjuv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3tpzncmph.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3gxjocwop.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mpjdpdiv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxnrbnxe.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mixfuvft.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpcrrqjb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyrowjzh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3zkyogqgy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qwjaypwq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uspenpdr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3sijpgmlb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3vgdcjqre.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mhgbxkxt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3znopjzcq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wnacgyfj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bkujlnim.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jqutyosv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3dfksonft.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3akxftlmm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3jbxwieqi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfukcihz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbdhutve.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ourtyfyq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wmhzceek.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3icepyecb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qlixguic.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3swomvlgl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pzlzbsqd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xbnoqwak.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rhrgknwj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmiudvsu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qstkwwxj.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3aucwjtlv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3hphyxcuw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3zcteblvy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yomooqpx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gjnwpvqz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3jweaueye.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3muvcmgaj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xdopixyr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3seaxfybe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bcaxfyql.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iincsdih.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3nuwkjxfn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lavywxod.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rhhcjgrf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jcweomdw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3qtdrbpfm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xvyvmxkc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3eyxnxblg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jenazxgz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uijawsfh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qzqicoro.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wtqsurbu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3avmgnpgb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ifivldgs.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tiacfssb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxlirxdm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxnrvxsf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fxpszsyn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3dzrsvlcm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3micihclh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3npxdzxvx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3nrlvwctj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3zpnltrcs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3jvgjvjuo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ihiywxyd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yyozbani.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wgokymsl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vgqtgesf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pxduxbsk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3eglaiwqz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzvlhpbx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3yfurgxcu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3kllepfmy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rxygbwyj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kmtcbprk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vzcylwni.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ipxlpwpj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wjxizbwo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pjuidrpn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ucwrebao.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uvuenkkl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3oyvymjnp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3rddxfhpx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3iobvgmtd.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3svdfelcj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pkcfounc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gsfxxfea.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hqnhcceo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fblrygkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvhyvdyj.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3gmqzfhlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkgzaptc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3obhsvkmw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eltoreim.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijbocsje.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3plqtmdvc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmqhtrra.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymvydpdv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gcfyezbl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3elfjgbwo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gqrfmnzs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uianijmo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ajdbcnds.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgdqpalh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ifahtyoj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sydrfgef.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3mnszfsub.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vtibvtmv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3muikdzcq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3pwopnpra.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3zlqctzgf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3axqeewtz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3smolpajw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xmuzusmc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewgloxgj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bvlftjcb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fojppdbd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ccozoanm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3onftkbet.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3lelrscxw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qwixgkjf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mlnwolyy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3grnehrhq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3yodjuhfy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zfhnotkx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3kdcqxwsq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhdtwsna.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xejlpzgg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3gwqtcxlz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3awvwagim.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3sgyuqogj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qhhamdzr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tndajwsq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3pvnmtiot.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yuulquqf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3divicmwl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hifbqlid.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ggdtyrww.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dooalceb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qvgabzhd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3huahubdl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pwlufyqm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dowodlgs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rpaakzdu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pojytfwp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kcpxvbpd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3cttdqsjy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3kftkbpbb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qusrsoek.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dcsxkloa.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lkudfwhs.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yeyzdbfz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xhfgochj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3chewmuvz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3tnooitus.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ofhflabr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wetcxdku.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3epphlrnc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3obvnrchs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ihestgoc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3yuyjourd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wnybcwje.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qxqlrkzc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3krbqzlhi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gvmonesc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fcwrpfda.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sbcfwjau.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fhealtml.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cansbyxp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3baaiqjwg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hizzlaoy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fcchkpcy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ejsvtovs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zbqxgoef.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gsvrkvrx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gwencpck.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yeqilxaz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ylipfwnw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3icqtexwm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zklavhmn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3muisjkxq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ihhadcqr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hkamyepp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ieshuhui.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qunifgct.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rsjpepuy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lxelwiem.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zmovsuky.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3baaecrcu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3eonsivzz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3qnecbdlv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3popcocww.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ghcvfiwk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3juznlhce.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tcmzkrgg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3icvrmdan.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wzzonyrh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3mobedfat.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3etazevlr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qjtfgpqf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3jgmiythe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wrxfxkhy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3otdfmawx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3gxojhxod.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3irildvmf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ikyfoeig.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yhwglsuf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wcidyzdo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vbauvgkm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lcdssfqs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3yxesjcdg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gtnfqzuf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rxgdpcud.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ievbmgup.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ccoxtluq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tcqgfdmu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hquhqvwt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zdryyilq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dugpnlsd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gvccmnno.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ksktwyyc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ykkbamqp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3yaijbnat.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kvkhrarq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ygjghrfk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ztslxjyr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ssgfyphh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3kxidrheu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rqydlvvt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3husqjiuj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hklnbrdr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3swqhkjty.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3klrsenwf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3azeqhiro.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gvyabhdd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hovmfnet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfjlljzw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pblyatbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vahrgske.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3opvldngs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mulunqko.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vuneygvp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yacdeihp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ngdebjat.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3eozqjbhe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rijryyfn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dslvhsgp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qooqmiui.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3npjkfrtr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cvupdkmf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3xnuveyzn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dtergpge.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ddbhtixx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ynqfqehd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3chyvantn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ilqwwafb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3suydjdsv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3cmtyitol.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3igjsuzdk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3iozkaeit.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3njfirrgf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mpxbaabc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bxgkszwh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hkkxwsba.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dxdxjjai.html


<!-- 参考信息 -->