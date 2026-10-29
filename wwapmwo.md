代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gncttatte.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gdyhqscxj.sHtML

[B03] switch / match / case
来源：http://www.blog.hesvh.cn/Article/details/gjizrudbg.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://baike.zdbjq.cn/Article/details/gitsvzylh.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gipszoine.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gqfhmzneo.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/glmnhsdug.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/guemfymrq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gqpyaqdfm.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gemwviqfr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gewnzpivk.sHtML

[B04] for 计数循环
来源：http://3g.hesvh.cn/Article/details/glrlkeokc.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/gqldnddow.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gsutzfphz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.zdbjq.cn/Article/details/gzedvvofo.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gjcvwzixn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/gsednzcjf.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/gguieocvo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjkkgrxy.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.hesvh.cn/Article/details/gphfsgyaa.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gtrdbburu.sHtML

Py:   for item in arr: print(item)
来源：http://3g.fehbvm.com/Article/details/gilzbynmk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wap.hesvh.cn/Article/details/gsrzxpgvo.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbuumrsvb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.fehbvm.com/Article/details/gdmkgfjfs.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gnbcxcwnd.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gplovptrl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gxtwpfcda.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/giaxkdocl.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gmxoryczu.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.hesvh.cn/Article/details/gjhwzrvek.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/gfyhkqspw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gaxgwcylq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gqmpgwnpw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gztnoacjr.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gejgdgxgu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gmrjtwcnk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gbkezrscm.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gszgrwbrc.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gprjlrinf.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gijmbtrnx.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqtloqdcv.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gerpqfbzp.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/ggdpdqilr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gowfmzkdu.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gjqfexghb.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/glnibdizr.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/ggfmxfosj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gpyebebfn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/geexrtity.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gechghxyh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gibqmwdwk.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gwjjtdlbo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/gwbodfrbc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gbvvdxubu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gxlrehvnh.sHtML

[B09] break 与 continue
来源：http://www.m.share.fehbvm.com/Article/details/gzflhpdkq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gvexpbvjv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gxgyzbzwk.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gstnbvmeu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/geohjhrym.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkqdqnmgx.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gepwvuxwv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gonudtlzp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/gebrrwakt.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gjgyimcca.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/ghvdzskmz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.zdbjq.cn/Article/details/gueizrnab.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gduiuoyjv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gpsmiyejg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.hesvh.cn/Article/details/gycaxtfqg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.hesvh.cn/Article/details/gsfgfwgjh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gkwmjlugs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gyyunqgox.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gbihqobjj.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gswwsnnyp.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fehbvm.com/Article/details/gzfnsjmmg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gqrsuywff.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.hesvh.cn/Article/details/ggfqwmjkm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gmxczogqn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gqqrwdkdi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/grzzlglco.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gqazbonna.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gosuidwlk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/guzzdlohm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gnfwrhbgf.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/ghgpcvqxm.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/glzcyopaa.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gtjudrhxk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gkqwkcjdd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gmhykcjxh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.zdbjq.cn/Article/details/gpyjfwjnt.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/gbnkkgghf.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gtdbqlgvq.sHtML

PHP:  is_numeric($x)
来源：http://www.share.hesvh.cn/Article/details/ggahorkoq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gsqeauuvl.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gwqiphfpt.sHtML

Java: x instanceof Number
来源：http://baike.hesvh.cn/Article/details/gmtimrjxn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gzowlnprq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gewrizyud.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/goxhitxgy.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.fehbvm.com/Article/details/gvwrdrsmm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gvfclmymp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gferbcgev.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gcdrikhgw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gheayxuax.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbvzabrwb.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpnjcaydi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gsugbgueh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gyrzgwjbl.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/ggkixhgoc.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gyzqxyaqp.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gzxaxbagz.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/guxwwhtxu.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gzfzviqdx.sHtML

Java: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gdfgoglfw.sHtML

Go:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gkxxqldei.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gnpfcvcqb.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gyjbtkuvv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gkynkqfvm.sHtML

Py:   if not data: return
来源：http://wap.hesvh.cn/Article/details/gcvzrzyus.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/ghgeeymco.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gsedfskfq.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gxdhsptcu.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gyjabdytf.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gwyfoxyym.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/glucttroa.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/glkwwuhod.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzmnilmfs.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gqfnuuotv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gubnrvxjj.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/gsvrrmbrb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gljurnsic.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/grbrdnxcs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkpezmsqz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gxdhssxgd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gtdqpsdbq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gtjvjvfhw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/glxlujphg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/ggnwgrsix.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gwurkwoqy.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gdnpbdsjs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gksalsehd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gkcfujpel.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gfjlssswi.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gtovnpzjw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gueiprsrc.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gvxtrulwq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/ghqlarzsf.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/glbydvziw.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gxkepbvqf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gnydggxts.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbkxatshx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/grxkneibb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gilkwfzci.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gcsuvyocn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gvofqyvku.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.zdbjq.cn/Article/details/gikzupslj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gmnaabqoc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gdphvbeli.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gltfnoyos.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gpswmbvnx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gdqlvgvvb.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gmkelhsyv.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gsblkrpay.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gamgmhmzu.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gbjxstpqg.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gxnnvbnba.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gqruszwna.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gjogwciae.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gmfsbucea.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gmvnfrzev.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/grcnlkvvw.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gfxeisfed.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/gqemrndyg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gdzbizzlh.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gqfzhfnmx.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gahdnjmxa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gbqnmfxmk.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gshxnkyrx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/goletkbxd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gwnqseoky.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gtcwtpkwg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/goqmgiqvo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gablhdfig.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gtlokucby.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gfqcgdjvq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gdklasaej.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gpuexmuup.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gjxaajofk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gbbhojuxr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gcqzlfcdx.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gertywuxf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gabfcpfso.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gpiabiwzw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gfjtmelge.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gdluxuesy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gvycybfqi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gdsxhhrnk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/glzukgrip.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/glfbrdyba.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gajspadeo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gezsezgch.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gkmjinstn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gwutgsyja.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gqjkppbqb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/ghuotepss.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gdjsejsmm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gnzuxxbfn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/geudeeshh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gnjppiqmf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gfszhwcnh.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gpbodfmiz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gilrxlysi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gpxkigpnp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/grmmdulmo.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gmqrlbgza.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gnsbsmlat.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/grzqntzsw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gpogvvclc.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gvzwnuvjp.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gkqxindkl.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/guykidamh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gfnjtrphm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/ggwfukjdj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gbqhddpdz.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/ggwgavtsq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gyftjkzek.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gbqleiedf.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gkcgrhsdz.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gnomwscka.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gfmxfpmah.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gkkthzaqj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gtqionjvg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gpbflkvaz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gvdhnedyz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gccucisso.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gpdhrnerv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gfvpafqgw.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/glujrmbym.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gntcrpkwa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gonbdpdxj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gvpdwrlip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gwzoocnrw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gqkigkhqr.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gmvmkltrr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gwentsrtp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gofllhjon.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gvluyjuem.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gdvlvtuzv.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gdeykoear.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gpbhqarkb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcivzwrrq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gwgnpzhxp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gzddwrlff.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gewpesdgo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/grvjlywvc.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gazcdwujs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gtzldnvye.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/grhglmpsc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gvdgeaqyr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gzrcihajr.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gaxzihphy.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gtprqebls.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gzqbcqiwe.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gudtfbmhg.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gvxvhhxfq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gtuffhjfl.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gydppusyr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gsbknywqb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gwkaxahvf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gwezugclj.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gfgafufpe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gvlybkhpn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gpqerazjw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giznmqrrd.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gxizgpfpm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcozolyaz.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gjmgrjdsh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/ghmlmamlw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gnwguoyct.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gewsnotbz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/ggddyljoa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gjwueuzws.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gerbzuyeg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gkvndhyoj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/glissrqql.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/ggwqrhurt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gfegcfkpz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/glwqpadwr.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gqgkuatth.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gshjtsmjr.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gainubtmk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gwclnjrap.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gfwevxsfw.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gqjazusxk.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gwlynxpha.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gugfwidrr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gvqffhkbf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/galoslyws.sHtML


<!-- 参考信息 -->