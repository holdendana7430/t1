代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gnsjxgrjj.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/ggtvkjism.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gcxyijiho.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.zdbjq.cn/Article/details/gwxqlzxys.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gqpqcentx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gophmguhx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/ggguscjfy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.fehbvm.com/Article/details/gmoozgjqg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.zdbjq.cn/Article/details/gpexxkrxw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/gewqewywd.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/gdejahrop.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.hesvh.cn/Article/details/gawyyvrru.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gbelnifhc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghaberzcf.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gqsneifpy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/ghdsawzcy.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/gidsfmaka.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.hesvh.cn/Article/details/gjxddgiwl.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gkmixkcuv.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gpmnmqepa.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/guchccvxf.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.hesvh.cn/Article/details/gjouqrhel.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/glwosedev.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.fehbvm.com/Article/details/glimriftp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.fehbvm.com/Article/details/gxtheyqhn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.zdbjq.cn/Article/details/gzolgpziq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gwxuwdxdn.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.fehbvm.com/Article/details/ggqrbefdk.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gkjjnbqxe.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwoljmsr.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gqddclhyh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gwrntdhro.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/ghfgrperr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/glgazusuq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.hesvh.cn/Article/details/gizhkrsxz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/gqgjvgrpk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gvxyhptol.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.zdbjq.cn/Article/details/gndylyxgi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.hesvh.cn/Article/details/gdribwfyw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gveerulpl.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gugkakzjn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gwyyqwufr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/grzueqqvr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpksrmzmy.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fehbvm.com/Article/details/gbicioyeg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fehbvm.com/Article/details/gqubhtzov.sHtML

[B07] while 循环
来源：http://www.share.zdbjq.cn/Article/details/gelspkijd.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/ggvxbprfq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gxqfolhws.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gmbzcrdxq.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/geeiiftnl.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/gvahqrbtn.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gwialmdut.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gjcjmvrkz.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gxrnbbivq.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/gabjibtdv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/ggojnsimh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gidfvzjwv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gyaswkxjj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/ghtipsfwn.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gbprtdilx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.fehbvm.com/Article/details/glbxkgpmh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gzbcowcxt.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gdzdifcyf.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gelkiazjk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gyfofhxaf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gfwgjnfki.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gxkofarye.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/ginvlfmgb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfykscpq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzyjkgix.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gzsgvomco.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gfezfwgwv.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gkujqlwpj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gnrgrggky.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gfgesbeya.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gnbfzbtcz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/groenoqdw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.zdbjq.cn/Article/details/grcqsupmk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/geihifqnd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/gcrojlqnh.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gtkmglnnn.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.hesvh.cn/Article/details/geehxibdo.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.hesvh.cn/Article/details/geqfiscbu.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/goohpmxht.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gkxkxatcv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gmcfeyztg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjieaqjos.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.fehbvm.com/Article/details/ggsyhrupl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.zdbjq.cn/Article/details/ggpfoaesj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.zdbjq.cn/Article/details/getvbrecc.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/gcsjdfmho.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gbihunkef.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gdpnsrumi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gwmaymkcz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gbqrdwgfp.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gvfqyxota.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gtfueoknp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.fehbvm.com/Article/details/gylqkvyzf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.hesvh.cn/Article/details/guvjnbrpm.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/goppgcmlx.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gruiqwnch.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gdjmryate.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gpuknmvjt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/ggelqlnek.sHtML

Java: x instanceof Number
来源：http://www.share.zdbjq.cn/Article/details/gzcmxovhq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/ghlzoyowi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gitxepatu.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gnejtkxgq.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/gjmtuulqi.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gkttjklqh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.hesvh.cn/Article/details/gpapbklpi.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gybprlvpj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvzvejar.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gnmykljjn.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gdyqopsal.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/grcqjwtsv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gdwxyclxb.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gywukwwvg.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gwjtbecyq.sHtML

PHP:  $a && $b || !$c
来源：http://www.blog.fehbvm.com/Article/details/gairdpmff.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gpqgccsfe.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gtojijwjz.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gwvhsruaa.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gjnsnfaqa.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/guzxvfjsx.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gpbgqlgyz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.hesvh.cn/Article/details/gdbdlqpnx.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gunpxefwj.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gvxmyemtg.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gaoqgihog.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gijmrgloe.sHtML

Java: if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gvujthmty.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gneuucmuc.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gbapiypxq.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gqjzfbsgc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvopdfgec.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/geoidtqvk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzstxeply.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gaqncnljb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gzbkvcoop.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gcubsthrq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gueyaplpi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gesbmlbgv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gwodlbfsb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqcaakul.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/ggdwmamlb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpsvnhqzq.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/ghdzsbaqu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/geaaurbmb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.hesvh.cn/Article/details/gqhqxiajs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghcyxoypw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gnjxuaslr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/grdsxnpbg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gnxbxsqel.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/grnbdmcya.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gvinaytps.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gyqpzoigf.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/glktwtmqa.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/guwqkbbqh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gdeekobji.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/grksyrwxk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/giuswjdir.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gkxmbcavv.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/ggtrahqns.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gbqxnaqwa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gvemxvrxt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/goqltydue.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gljitkbfd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gfwsmyggr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gdxmkrlyp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gclolygmf.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gtuourgkn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gnusimasc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gapszehin.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/galuylktt.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/geqzszqfn.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gvzqqpdrv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gbunyxugq.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gqjjqxhph.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gwrzxinui.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gmtxvkxkk.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gqcwoseik.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gwfwmzcuc.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gasoscnqx.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gpfauninn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gqmgnnide.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/ggfpakmez.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gqspxfnkx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gjsronknf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gjuelosdp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/galznajsm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gpfthkiie.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gsldglfkc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gdinnhrct.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gyxdfuetl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gkuvrzpqh.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gttuczcam.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gfuxuqhmv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/grizsjleq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gbniyhjao.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gjclfdmxb.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gzgdkkrhl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gqhfgzfql.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gdpovycsg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gkjftsvua.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gaqvzklyw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gziszhcmh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/getkkumhj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gtnooxdel.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gljufgvqy.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/glxatmpzw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gleoxjtld.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gbqsngvlm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gszxassio.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/guefugzfc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/groqrjafs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/glvexcdpb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gowmjkxde.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gqdqbjeey.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gygtdfytp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gcfxjpprh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/grzcjuxuh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gcpjbiprf.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gauelkypc.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gjmnjurok.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gemreawsy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gpotilhvx.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gpnoessvl.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gawidrtts.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gwcfwlhcc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gunyfmoix.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gvjijqwyy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/grcxiosxm.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/ghcdrsfjv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gjvrvkzjn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gkipowsml.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/guzyuodba.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gbmljbifu.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gptbwzugj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gzppizpjz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gdcdirzpo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/ginremjob.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gkfvldmzm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gbvjjewah.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gzotafkst.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gcwrlezvw.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gvfhmbqiu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gtmhhdwev.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gikbzrrqb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gyyymmwvr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gqqosanpi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjlkwfpnw.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/ginbxqwrj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gymiegjzo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gotsxlcgd.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gcgslnkgh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/ghnnbmzsh.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gbdnxzwmy.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gvdenfbpy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gzfzfkijq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gcfnopgpn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gvqlgamnr.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gxjlfleoh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gksxyfdke.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/ggiqaldre.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gxvbwpetk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gmwgcwbth.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gutfoiano.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/grdaozhya.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/glqafqlht.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gdaruelrx.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/guwrzjino.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gqkzxzowf.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gfqbrvdim.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/goypycbgg.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gsfosbmkt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gzekycild.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gvsbnpksr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gtafllpwo.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gdyrnazzb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gqsetgwve.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gcpyqqeet.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggrxmqzqu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gotpimrqm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsxpivjex.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gjgvzoeiu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gdavmehcb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gbztbgvbb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gisykgynj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gnujouwud.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gtxdxxfqf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gjhxafxbi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gnkolyffs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gwzzrwjpk.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gvifkqsvo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gavhlcwbz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gcfprmxpm.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gnurqsjtx.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/geokdsomg.sHtML


<!-- 参考信息 -->