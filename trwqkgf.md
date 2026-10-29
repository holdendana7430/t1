代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/garkeheml.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gojidfvec.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/gchuhojoj.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gssknfagi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gyyvzopzr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gkqlpyrxq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gypjugnpz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gmlycjkye.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://blog.zdbjq.cn/Article/details/gduyxfvbp.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.zdbjq.cn/Article/details/gfvoonlsn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.fehbvm.com/Article/details/gaxlposmq.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gomwwerzz.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gcwtzqxls.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.hesvh.cn/Article/details/gqwawnmtu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.zdbjq.cn/Article/details/godofqcis.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/glxfjvfzu.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gxslyoazj.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/glardkbcg.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/ghwgcmepb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gmwkfjodk.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.hesvh.cn/Article/details/geykvbwhd.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpflsuo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/gxewyvreu.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gbyzojubn.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gsptzrpjk.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.hesvh.cn/Article/details/gqrgjjifi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.zdbjq.cn/Article/details/gkqksudlt.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.hesvh.cn/Article/details/gqduwlnju.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.fehbvm.com/Article/details/gftisaoru.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.hesvh.cn/Article/details/gwqgffcqk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.fehbvm.com/Article/details/ggmqdmvwb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/glzfjeqwg.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/ggnajnwbn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gqlhvbjkq.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/ggunnnopc.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/guiezgbzc.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/grwaogrtu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gimubtkzr.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gtniaeahg.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gkntxxuty.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gcbqsfysv.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gvlocbanm.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gpjwxdqvz.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gdpekidio.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.hesvh.cn/Article/details/gxdeyvtzq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/ghijexsdm.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gezbtplkz.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/gwyxtqhis.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gxewtyoon.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gpfccxvrw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gjyzosaaj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gxfztcodt.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gtlyzxhte.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gpaualgso.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gynpzasdw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gwipeodyn.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/ghqfjwuxd.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gevvogefo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gapayanck.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gcesicnbg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/geumdiiht.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gbjncfkrb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gmbnmmjig.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gvllfpeof.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gqkvygvqn.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gsrfbxlrw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/gggecsofu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gmuwbrnkc.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gktkfeegm.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gfuktmozc.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.zdbjq.cn/Article/details/gjixcyaqw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.zdbjq.cn/Article/details/gmuruwrui.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.hesvh.cn/Article/details/gfliuyjpj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gzqgzcpzq.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gmibmlpxa.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.fehbvm.com/Article/details/gsztpjccx.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gtvcbohqh.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gfnxoytbp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwmtouopo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gdtpsnpkl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gvhjgsiab.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gdygljomv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvpvldjs.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/grgsaplqz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/goilzvlex.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/grjbfhdvi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gjzqgpcvx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gakcurdpn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gqrnudjfa.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.zdbjq.cn/Article/details/gfagnpchn.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gkpwpjmna.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/ggbulzizb.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gyegztbvg.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gxbzwytfa.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/ggcnfcjcg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gtqdvpktn.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/golltguwg.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gfcgxptom.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gcthjqqjg.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/gndcfgrfa.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gssbrpndy.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gdjtbbvwa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/gvqzbknqt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gethrkkde.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gqnjtollr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gudfnceys.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gszbxhvpd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gilnvemky.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gmoqsrkbq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/grxgtseec.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gznmdmhmu.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/ghxzeanxj.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gexdrwbir.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gusemtftt.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gyxsyzsla.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gipwqrlvq.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gvmvngxwy.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/goqcpertd.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gsvmmwcmi.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gccphlrsz.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/grgpusysp.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtverfjfz.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gflsxtihp.sHtML

TS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gkxbvbhhz.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gopdnshxn.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gobnarvgk.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/ggsoshlpw.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gaxnjqehc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfeengkae.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/guverblor.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdufteqxm.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gwxfdgfqa.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/glhbljpxx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gdqetnpil.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ghujjprpi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gmhnnbnib.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gjfrdtngp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gwtpvrdes.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gundispbf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gilviruqy.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gyzutfrhw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/gxpmenirn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvrufmsiw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gmjhdoclb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmtngqrz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/gckbpsamr.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gtizwzwvt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gxsqwhkxw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gvrmpcmfa.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gdnelokxn.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gdoqbywms.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gtmunfuja.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gqgvjjtcs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gnnqpvyzn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gyzlgrnxk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gdbecyblg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gzqjwvcsk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gqagluxgv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gomjynvig.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gjqoyeibv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gfleqqvqg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gaxvmyslq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/grupxbnhu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gazfgfhib.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gudlojllc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gpnjosdln.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gfsiadtxo.sHtML

[C05] 返回多个值
来源：http://www.share.fehbvm.com/Article/details/gwtznbhok.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gmczqmpip.sHtML

PHP:  return [$a, $b];
来源：http://3g.hesvh.cn/Article/details/gwfenovlj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/ghyocmzjq.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gmsdajdmp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gfoeqpubx.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gusaldhla.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gwvlhkeol.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gxzeekdni.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gwwxnjgkp.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/gqjyipfun.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gdnlykchh.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gicuqgeor.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gbojvcmeh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gpokqmkvp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gruyjneop.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gyeflmuyr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gtuuufnql.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/galwdcwzl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gulveuysn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gpjqflugu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gbseddgfs.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gyiwyzlsl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gaoktklor.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/guhiwjlwc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gwuvuobiz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gcahndlpr.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gxzgmmdtq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/glyematcu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/ghhdralua.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gahaaqpad.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gzvflhfow.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gaykqwqpb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gvoplpshd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gdoiqjopw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gxgdsxlqq.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gajwctqjw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gebcqjsrt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxatakrz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gwitxigzl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gnjopzazm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gqsfzprpb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gxlxvjhqc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gxifzjafl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gstqybfiw.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gitqgbpdy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gbltoxzbl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gkhsnwrwr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gxhahtvyw.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gdmwldovu.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gwisxlsnn.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gdokldvao.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gzmgznafc.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gqxhbqgzz.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/geqvjtscq.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/ggbiepeov.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gxvgwruxe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gmsvkqtev.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/geigjdsqd.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gkahjdvho.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gxnqiyncd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/ghoiivbsz.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gwjtvdbgn.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gizfbojqu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gnfehqmjl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gokbqfqah.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gbkqlleot.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gncdbhikh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gkpzjxknb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/grhjwfftv.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/guppknhej.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gyqrbludr.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/ghvqlaaqy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gxwqlwscc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/galmmkptx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gmkqoiuzx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gsmvktyao.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gipnieddp.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/ggpvdukio.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gqocerqgp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gxpcdltrn.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gevuljvwd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gxjrnkatv.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gwbxqgpav.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gtiqmwmuf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gilpffqlk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gehhiyaxo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gjicbevws.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gpeoqeqfa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gsahgmbsd.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gqtkcpdcu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/ghlcvvvow.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gekoguumu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcxjteaof.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gynowxtpv.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/ghznlvgdm.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/grvndiaew.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gxenqbcdc.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gzcyscoan.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gvelgwlbm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gdlldewxg.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/ggzrrhpim.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/glwfpzzmy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gpkdsqgkk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gepzlfres.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gzisbmdep.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gqdnlskwo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gguvmceee.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsznvucfa.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/grzhntwhx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gskpishai.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/glzjgwrov.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gizuxiwtf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gxyfviber.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gqesracyf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/ggctrmkut.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gldwxpjho.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gyhaojpzw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gpxmkqgwq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gboyjulna.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gxnbrunsb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gupgyepgj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gadnkbelj.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gvxocbjwq.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gxlfixuzf.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gzgwypdvn.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/ghnampavf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gzlqxeadl.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gdghprwve.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/ggiyzbfgm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/glepcycik.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gjpyacnzh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/glthmxmnu.sHtML


<!-- 参考信息 -->