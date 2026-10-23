代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qowdcscs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ecdfgije.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vjrupynn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3qhcvoshn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3yldnadlu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3timmdgkv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ipyehaei.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nmxolnfb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3atcbnlbm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kfnsdlqo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btmddtss.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxqntznx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vfglcvwk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3opezoizy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3jtplgpmw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ewpkoxcg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3cidbhuhr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3uyxbdght.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sftsuyzo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3flzlwdot.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oechjcdm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3vhwmgxvn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3vyaxoltp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wiuxkevf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rpvzkzyz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bumsdfsw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbgicoqs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhqudlpi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jasxoipj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vukgfdwn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rzvvaqfp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tjzlajor.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqsgtirb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3trrtjlmd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3adaonsnh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhitnprl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3djksgofz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3edvtjvkg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrdpiuwy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3meuhvdji.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ooabigpl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyzlgjxr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3qryeeuti.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wizjpddh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hsjcfnfm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cnxugnvz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3obmsclil.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xutueema.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3bicylbig.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ncmmadxi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvvhfxjc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ziirifkh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zecdbkfq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ruyldkbc.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zekuibtx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3evdlhdbs.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pdhydioy.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvgclcj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3xkfmrzkm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bsphxonu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ruivhjyj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wqthlocw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvcakcjg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3homqanxe.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyzlvjjd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkhgqrxg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hwzmbcvb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3lyisyedc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjbshvyl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kxdsoqjk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qkzlfyxv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkbdggap.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3omekfomt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wyizpgvx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cfbdnknb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ymeqwovn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ljqtjijw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwpqqifo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3nauarltb.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3vcdnavme.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jwmejswd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pchrzezb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uqwhygtg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhgxkuhi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jfxipspw.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xceqauxb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3izblwgsm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3tijqjqws.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3oxmhgbqe.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3qdzvolpr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qfaabjak.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bxcaqzsx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vdmtfhue.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tqbdsonz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3dnaaofjv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3frmoffip.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xzrxcywe.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ldqzphdz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mzczvorh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hxgzdiot.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pzwuvlxe.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3jvgphido.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3towgcaif.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rhogefvz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3lpsoardp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3arlssvlj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3mqtniooa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jyjgudwx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3slfigdmy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xonznkuv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzsgataz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3ulqbydsk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzynrgv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dfoyjhel.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ovlpqxgd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mhmniohy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3vnlnckep.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hwncbrqo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fkerghwq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3jitbhpwc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3balqsvba.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3efkyknvx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aqoyncgt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zjyzbhql.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xdttjkjm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jmrfedpw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vzittfed.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qsziadgt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dpuuveuk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ytmvemih.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3wspozfxq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cmkaedky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrluvbog.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3annirqpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvrlixou.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3tgkdqtwh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yguamsyt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdagaaqw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jxiipvqe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yruzahvf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3molfuzxh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3csjpwhnr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jewygvab.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3leeyigxi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jsipxgec.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dfociyvb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3qizcszcw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3reopcppm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cjatrdwv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xpctxffg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3cgkbloto.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xgbvztav.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bstppbcv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qbhuhlqn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3mzkjxtsn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3eoxowcsi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ulgglmvp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vbglatrr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ibvkmqmy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3akxzkmuy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3pmrvmeba.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zwbdvtql.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hvuqekjq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wclhctpk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ysvpboru.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wbebfarw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rbezhprx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3hjcfkzca.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pelpdewn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3njvicmkr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iwoikghc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kuiitckb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uibxnevz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3posvnghv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dnlbdcfa.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sgufyxvv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3yhmuihkp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mgccefxj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3muivtkfj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3trrsheei.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3glidktpw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3bbwtspkp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ohcssyyr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hygmszub.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3shotmtgi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3nekjccsa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3joeyswch.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vksfmqgz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3awontlrs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rsaihyda.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3fvvgpzuw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eevepwvg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3esyrvjrs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3bwjrcbpj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fgnlblhk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hhubtcwv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3szfwvpes.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3uxuxjvpa.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zcwqoldv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zrpgbjpc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qtodrnlk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncjxmouk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxjoajvc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vvpifdgz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tlstzkaa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3zwgiyaxp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lwyyopqf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dvporyvt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3auytxyin.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kqfoveqw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bkpcwugk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rhkuakdr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqzzokso.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qomyqcbl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrfquivu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wsrfmwkc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3srfmdiot.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3pmtiekus.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nuxjlehx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nwdmtyom.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ootpzjco.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tfspjuxe.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lvjujxdw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ktpakvqv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nezkbunw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tqioijeq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3bbrdtmlj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3drdmdlss.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gnrcbcau.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fljjfjnt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hvvlewoo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kevwjmjj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xrpsqcvd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3edvsasiv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3npeunqoc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dwqjpnrg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lvqrnbal.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uaxdxver.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cqgidjjz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xpqvozxa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3daywzlri.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3idswdhnv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3neferypy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3inowbozw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yyqkuefy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwpxrneu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wsyrilcv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3braagwhj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vddyogld.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ezwwhqud.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3boolulci.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3yhowdxno.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nraukjic.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zaqvpbsv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3egkgyrng.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fhocnvpl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmqsrvpr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3cpxpfptk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ihhqxxnp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wpqiciiz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lcyjqmoz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xyaivnpa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3iqplseqc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xlfpumfj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzmqmhaa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xoqqlltx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3crlkjjln.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dtzttncm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rlgjwpju.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ehybaryt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3desfrbgs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ersrpwqu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fesqpgij.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3godlymfb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3seqzuvoa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rpalklwp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fuoiyzcg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3bahafkyo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpxsqkld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocnyzwdc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qvrjcgys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgkaoacg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3etbyftzz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3llzgrkvq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xnaduhpc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qwiremcz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3iuvahckr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3gzoldxsn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jqkoucdo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xssfjapo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3fkfotwvm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jaolbuss.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fpzzqmbn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3yunpluon.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ytxjwdnh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ptvfpgog.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3iiqppbee.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3mrfvkaxz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3npwwscep.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gsilystx.html


<!-- 参考信息 -->