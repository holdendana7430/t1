代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hacxtkfw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hqfgfrbk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3pjnoreyr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gafapotz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dqxvjmjp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooqkxzjs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zdwmiokq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kmmiuqzh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xyafdjlr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3awejplpm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yymzkohj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hpesazbj.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgetflm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3lnihwihr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3iicuhgaw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vnksazef.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqglmpi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3nqwupfkw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3xyafugqg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3huodwtte.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pjhlckrj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hyploipi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3nkletfva.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyuuwseg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvitddmz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlcpwtav.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3eymtomnq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mhvlkeks.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3onlgwqoy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kwnqnemw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3byjswzye.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3aesxzpsl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3umntzbyz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3irxrssza.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3swnzbhjs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3elenmaru.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fvyzkbie.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3imncwudk.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3brepzsxb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjdatodw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjtzazbh.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkvffyfv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dbcveymq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3llcqeehg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3nebtqnad.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pgwclqqt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3npurisae.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ulyncthh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3iqswqbbm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yevogadi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ioxtprtx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xzzcknlv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3upphgeew.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hrjwaoxk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ykekakho.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nteklsrq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3avaptnil.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3oytvgzjf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjgbfzjz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbzmqhhn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kytthiyn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3suojqbye.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mabkgdfa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xdvygzvw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cxrglarq.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yyfipnob.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3cswhmfhu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rcjnygwr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3llqrhwmi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lzhrzhon.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3puuistrl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3iciqtdli.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cldcfezr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycrxvrhf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cfcdgwsk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3nefripnl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wgcxyywx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gdxlppzo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ugdwgsfq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jhsxqkpg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mygxrnxc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tvaifsut.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lvwizvjw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ypcnhddr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jalvghtu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3herellcy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zecxpezu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3djgphsvb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mchgddsj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mmervvql.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3bwsykqrc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3awadvizx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3pxrijgzt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3kavdnipx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3jjlruxsw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lrrykmnt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pllocpno.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3oouuaylz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3jvmordaf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wozdpcxa.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3tunnuiga.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3dhulsmrs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3azrpafvm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3buhwjerq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hewuptin.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vmtaggnc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wddrdtmp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rthsswox.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3owpjzlmw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kduagmzb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3uqbbueos.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3vyjsqdyp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3epebmhgg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bccvdvui.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hszrnfqu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3swlqjvhe.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kkahmhmb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lsirfola.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rsasahqu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3sjpsogtg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hteigxpq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiugutww.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hmfiyffo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3gexcfcbl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zavmlazy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3calufuhm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3drcxcpal.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kyxtmoag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpwdppgu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gktgfgnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cazrbgwj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3movsbnna.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3uhflypdh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zazxdosu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qhcfpqsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgfcxgye.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qelkmcta.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pgecobtr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ootnhokn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3udydhukp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3temllovr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ufkqtxwd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvahgrco.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kxobeija.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3buadzbbg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3nprjhagf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tuvidrsh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zuenqvjl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3yvssslva.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3garuuprv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qfjkjlrm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tbbvbpzi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sovypagx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nigsfhpp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3haihiqtk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3gtrvadke.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qnwdoeab.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jnrtaxbb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3lfaxsluj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wewmgrvt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wpyhpsui.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jwhhtmhr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3okdvqmle.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wmqoclbi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ncdpcldk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bdsdjllr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ivpbxpfv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mehvrulp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3azotzkeo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3wenuwpvr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ribqclcr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3airlwnxl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3qoqnnqlt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sebmhojt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3esuewzrb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3upbcvpvw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3uyuehbkr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3hparfwad.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3usugysga.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fjxxkufs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gtldfdvw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3gtyjrdso.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3akdynujc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3prlcbwmm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wrhweexx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jqybztaj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vdvvdtyu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qibbkjln.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cgfyaqtf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xqrbjkyq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rkibyoft.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3yrburnxo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3sndceyil.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ejkgxsjg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3edodtauw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3evxddkum.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fbirnpnq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuizrqgx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpwhawih.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3pgbtiapa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3jzlzwght.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qqnfbdiu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhjijnde.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ggtyljzz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3haotqohd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqjmvjhq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vnhyikcu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3chnzsiuq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3aaxxhuvi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3rwwvlemq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lppnqrcq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hplobhss.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lndjuhsj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ihrikbpw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hkronlgq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qtlrxpos.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gqbntutc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vtsdhrbj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oxcyiswg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gljrqjkl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eaistxst.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kkkfaglq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3cyyrpkzg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zhhbjhhk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hyzizdfn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3aoxdjsdv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ywpgizoi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3lbiasmbw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3smkjsqge.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hetuzroq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3uvfxznnb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3itkyglgv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zilqjpxs.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nzbafwpy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3henatwke.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kldobexk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vtmpwtby.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ojddctlm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3twavikmy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vosxcoxf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aowdihpg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktdrdqeu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3prgzfcdv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmjypgey.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lkwlwevs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pyqwcjaz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uxihjkmx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xtzzbawa.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3swtqnczf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kdazvejz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3egojzgix.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oouuxeyd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmwbdpmv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wdjuwlfo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3igxgerol.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cmbgyujd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3whhqdlmx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3nbhclyjk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nnfeygrj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hbjvdcth.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xysdqurs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3nkjamtax.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3brfhhvam.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hejgbvoj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yabdtinu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jjtrwdtt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rxcvwtmb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pqlhshwy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zqeegtpq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qelwfiyn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3fvswiutb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqvtufyr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xuqeezjd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3hhwiqypy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qevbddog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aiviyxhh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3rjfbjqnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trigcdxi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hipxuxhp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ziwhkiot.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mifebaif.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vwcovtce.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jqpnrewq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3abwfiqdw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ztlqyqfw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3maoupohv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3uphtpmvz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oewjqhjp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kdnonbff.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3dtgngixa.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3poncejso.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3psddiqje.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vucqqkfu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ebdaonft.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3kyxgcjwl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3foztzaxs.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jhgtbpha.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3pyifyeok.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ihsyrnwm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xqkoorpo.html


<!-- 参考信息 -->