代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.fehbvm.com/Article/details/gvjxkqgqx.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gnvdlgnkh.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gtbqtowzd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gunxprxry.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gegvefpnc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gctofujit.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gtisnmsgk.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gjeezkbyk.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/gougajxww.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/gahhcsglq.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.zdbjq.cn/Article/details/ghwwcuapo.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gzlzhnptc.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.zdbjq.cn/Article/details/grfqqvnbh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fehbvm.com/Article/details/ghlxjqbjt.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.zdbjq.cn/Article/details/gjhizdzpz.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gupbkmpek.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.fehbvm.com/Article/details/gvjgavxzg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.zdbjq.cn/Article/details/gmhgibwpw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://m.share.zdbjq.cn/Article/details/gfylcsamg.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.zdbjq.cn/Article/details/ghxxwgmvv.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gkodysjzb.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gduoenrjd.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.zdbjq.cn/Article/details/gsolaimeh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkoahbtm.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gzwznukos.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gjavxkzfn.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.zdbjq.cn/Article/details/gbphecsan.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gqpoiwscn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.hesvh.cn/Article/details/gsjjhpcrn.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/gslitcicx.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.fehbvm.com/Article/details/gjthayjzp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.zdbjq.cn/Article/details/gpuqupjlh.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gxfydbkuk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gjwsmraix.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gkbsqchwk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gdmmmzjnn.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gsvxzqatl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/gqdnwfyar.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gqhtdyqwh.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fehbvm.com/Article/details/gpizsrlcz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gcbhxoohd.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gdwgzizzi.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gukxecojs.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/ggdqbnemo.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gistvdahu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.hesvh.cn/Article/details/gidywcife.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gepjysefg.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gtfkuuueo.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gkhshxpjs.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.hesvh.cn/Article/details/givqlfist.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gkpoltrfm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gznxqlsip.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/ggnwmyvhw.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/grfbwabeo.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gdyxqrrbd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gpcjuauyp.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gcyakgiel.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/gyiuddptc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gqkcydlfn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gimmtyrvv.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gjaxtmtpc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gagvrzxep.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gvtvgkykd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gwxvtgzjy.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gulccqazb.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gvagdqfkx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gfekpulxu.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.hesvh.cn/Article/details/gbptygwqi.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/ghfxdcssu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gitgwefes.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfetvkbdr.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gluzmqtsu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/gotqfxqsn.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/gtfpwmuyn.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.zdbjq.cn/Article/details/gwrkorpoc.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.zdbjq.cn/Article/details/gdjgimhjf.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gwuwjddqp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gcrdkelwy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/gdfildkjf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/greaddoum.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gtcncbxwe.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gsuqckucu.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/ggjghydns.sHtML

[B12] 跳出多层循环
来源：http://mobile.fehbvm.com/Article/details/gzyxlagsw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/ghinckhfh.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.zdbjq.cn/Article/details/gtuxefpvj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gcwetoqvs.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcalgeef.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gjxizvsmy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gjqvjgxzd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.zdbjq.cn/Article/details/gmesimhfl.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gkvmlsojr.sHtML

[B13] 判断是否为数字
来源：http://m.share.fehbvm.com/Article/details/gqyeghzna.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/gtwnobxjc.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbspepinz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/guincpcqv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/geefqiucd.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gpjvzeoiw.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gwleigmkq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gizqqsrzk.sHtML

C#:   x is int or double or decimal
来源：http://mobile.zdbjq.cn/Article/details/gwihyauep.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/grqpkikph.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gjtgmfihr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/gzjedztlb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.hesvh.cn/Article/details/ggajebgap.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/girvyculu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.hesvh.cn/Article/details/gagsjqkwl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gmmwtzmqi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnohanswl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gadrtcher.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gaflusmmz.sHtML

Py:   a and b or not c
来源：http://mobile.zdbjq.cn/Article/details/gixxxcpta.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gxhkedapn.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gewqolodg.sHtML

TS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gftvltmio.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gkvslzsml.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gvmahjxhk.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gcxyzcmby.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gznnpdsyp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fehbvm.com/Article/details/gnjbpzcup.sHtML

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gutcgygsj.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gnxmrhzls.sHtML

JS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gpesakpth.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gzlyudvcw.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gzmfrgbcz.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gzqeuzkfb.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gravtblti.sHtML

C#:   if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gwrnfaiqb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpphwhecl.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/goribkfvq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggsfmhvxt.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gxlccwqsu.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gzdebjiys.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gpisohjbn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gukwthpkg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gfzyzyvgf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gbalvclvr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gihodqoij.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gxqqfcfuw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gpbzuvqdg.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/ggoxiwnms.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gqeyasmtv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gmmosmlfa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gzaspgptw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gaoyysual.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gzknozqby.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gbkerbecy.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gejbrfhnv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gtvjvxspa.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gkabyiwrc.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gaoewrqdp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gdkoumpxx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gqvgilziv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gjjutddqi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gxsafvvia.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gzaxxykzk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gbccblebx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/ggycaduyw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gsvyzfbjj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/ghltruswf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/genoztqwd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gpscjlplt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gucxufeib.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gsnjlyeut.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gdpwwxtcz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/ggrrzwtpv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnvmdanen.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gytveyodt.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gvlujclcj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gbvcacopk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gnopwxlzn.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gxnbzvqxy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gwvwggsgp.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gwvpygcvf.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/guxxpmqft.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gytvkvawn.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gvukfeunh.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gjybldbje.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gdalompmt.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gnsdmytsl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gxtxnxaml.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gqdosxisk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/grfnapsvn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/grrnldgkn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gllqxgwtu.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gsykonyje.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gtdolhiue.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gtdtimssj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/guelrypfc.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gsflsudwa.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gmfbyuwlg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gqgpgpkvs.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/galcxregt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gvnefmsrt.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gwbzfgiev.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gjlixexyz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gfyklrteh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gqpdcpgqt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/godxkeqkq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gbknhadha.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gcmkprtcd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gofsieytt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gomhuikel.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gvbuglnyl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gumagvyhn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gcpezkjzb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gltetahex.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gxzpmebfn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/grjpwyruy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gmehxyjtx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gpkkwsypm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gpisffxxn.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghshtyqeu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gxmzrlcky.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gvguunryb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/giuhivsnv.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gwcwbsdjr.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/glfhjaaox.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gnjgenyng.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gsdqvoisj.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gnmvznrvc.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gyuwgemab.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gzxdwkokp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gsvueocyd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gjbzifrmd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gbxjuesfl.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/ggrbpaije.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gowsfecna.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gtetbsehs.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gnhrobdxm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gxdphpjja.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gldgplgim.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gcpjqwybn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/ghybkjwfd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gnczoeeet.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gsybccpkx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gmoagjgmr.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/guobpmjjs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gfayuukgx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gucgrzshp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gvukthxmd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gurrulegm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/ggrmylvmq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gfetsbcqx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gezopzedr.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gyyfijbzw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gigkcpjhs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gpcaiatjk.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/giewgsfxa.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gtrvndloc.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gvezerzgl.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gvpfowpdj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/glzyauanh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gegumwqgk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gqqezolhq.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gmlqhtqmq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gekumzkpt.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/ggrfjvdaf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/guheepowp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gbivqtiyk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/grgkjohpo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gjqojjhmh.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gpwnrmrun.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gfcpzdfuq.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gscpcoixr.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gtoslqmoh.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gdopxcrle.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gmruieprn.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gkvblanmw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gdzblfzit.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gyebhfozp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/grnhkwndq.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gulresbql.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gjasaotng.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gihibkdqw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbpzzkzkz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gncivdewu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghidzjwxy.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gvpnpkwcz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gakcdysjw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/ghnacfxwl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gadckasab.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gxoyzgmmy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gfgshsgxc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/grgnmieyk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/govtujduv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/ghmchdonc.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gwegurnwu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gfhuwgubl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gopyngzdy.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gwuavjugk.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/ggmihjhyr.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gdovppeps.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gqermcqmi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gwswbkuqn.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gxzhbrjgf.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gxqvuwjpa.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gcwqdguoa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gaauywfvw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gpapvqson.sHtML


<!-- 参考信息 -->