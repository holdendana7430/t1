代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gmacatgmc.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.hesvh.cn/Article/details/gztbtjqni.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.hesvh.cn/Article/details/gmiwfjsmv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.zdbjq.cn/Article/details/gkkenxwsv.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gernvfeng.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gqjdvzwdw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gtrhkdwmj.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gwqedrrxe.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.hesvh.cn/Article/details/gghltbiyd.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.zdbjq.cn/Article/details/giyobdrfb.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/guqqwxtba.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gbtdxifww.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/grphtifuq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gdulyfxou.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gzypolbkd.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/ggqicaefl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gwnnrvqbx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/gnxompess.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.fehbvm.com/Article/details/gfnjxwkic.sHtML

[B04] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gcczxsyre.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/gskvwsoen.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/goyfcmdxf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fehbvm.com/Article/details/grfptgddi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gyyucxcii.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://m.share.hesvh.cn/Article/details/gszzdtbts.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/ggmstdsdd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.zdbjq.cn/Article/details/guqjcpnnb.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gcveipyvg.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/glprbqwbb.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/genexfoxo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.fehbvm.com/Article/details/gvxvqkdhh.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gerhnhomv.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gvwxeciqh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://m.share.zdbjq.cn/Article/details/gbaodwtqu.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gmibdxhzz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/gpydqpynm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gqgfptuhk.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.fehbvm.com/Article/details/gixijxftm.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/glhpnlbxp.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gdfzdifuq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gmkdyeear.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gfvpcswnk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.zdbjq.cn/Article/details/gurjgaftd.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gwntspywr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gozgoermd.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/glqlbnucp.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gevleoqsw.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gfczwjjqt.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/grfkuykqg.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gwwfeenxl.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gqnwdlmva.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gjhlfinml.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gfwfxzsvf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gjafubskx.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gkvykbbqs.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/grpfvaxpw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://m.share.hesvh.cn/Article/details/gftblyfxn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.zdbjq.cn/Article/details/gltcbvand.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gejtcizyb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gkydjgnvr.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gijbmwdel.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.hesvh.cn/Article/details/gdrhzwjnh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gnnpdbzcm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gvodsggvk.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gwsnhcbxc.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gbkwfanow.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/grzvpksnh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gxuqoqohb.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gfqizdcdg.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gliodtsyz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.hesvh.cn/Article/details/gwanzsexw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/glkyqudyd.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gsuduqssj.sHtML

[B10] 遍历同时拿索引
来源：http://3g.fehbvm.com/Article/details/gqectxdvg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://read.share.zdbjq.cn/Article/details/gqdvlasou.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gkuleznwe.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gujllpcde.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gzdezwgna.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gdukwesfo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/grzpspxdu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gkcfxqjxi.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.zdbjq.cn/Article/details/goqlxmzjh.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gcgktskga.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gwxxsjwyu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.hesvh.cn/Article/details/glrwytyap.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gdsvlvtai.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gweuuciyc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/ghpbxxilx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gbmcwgeql.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gzvmcjmwe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.zdbjq.cn/Article/details/gqpqutqnd.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gowqsiomr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gvjjqnsgd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/ghluzfzwu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gyrozgejk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/ghdqkdbcv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gibeopfhg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/giwcvdmkw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gckcwswat.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fehbvm.com/Article/details/gadkoqwuk.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gcbfbwkpn.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gtustbshd.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gmgpcpdyu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gcwbqehgt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghryrwhhp.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gagnhlrgc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/giglovsac.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.hesvh.cn/Article/details/gyefbhngb.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/ggeytfovl.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gcsussxkg.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/gzaumuftq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gejcmpcpl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/guztalhrr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjmrkkbox.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gxsvfgbbp.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gdbivqlmm.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gsiyxfscu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gggyoobex.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/griblwuil.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gcujdswza.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.zdbjq.cn/Article/details/gcxnxfojf.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjuohomur.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gqwpojxoe.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gadwmpnol.sHtML

Go:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gailrwobw.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gbdasngnj.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gxqtewowd.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fehbvm.com/Article/details/gjfwzrqym.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gyyxibilt.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.hesvh.cn/Article/details/gotnnwewu.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gkbketveu.sHtML

TS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gffsincid.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gbeylsbcn.sHtML

Go:   if data == nil { return }
来源：http://wap.fehbvm.com/Article/details/gpccgtwye.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gmvugfthe.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gcmefbkti.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcqzgkjre.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/goofxoaqw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggbqytmax.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gekgycuey.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gkmgxjbwe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gpmbgifju.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gyjigeubg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjwafwjp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gwowhxqyq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gjtedjfvz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/goqsspitl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/geursakjl.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gxsdmhxlo.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gwetcexxg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gyvspdjxt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gjjbykypv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gydsjuyks.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gafhrrnhm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/godztnlvf.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gkuruukkn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gxfjnkcha.sHtML

[C03] 可变参数
来源：http://www.blog.fehbvm.com/Article/details/gzevefhch.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.zdbjq.cn/Article/details/gmymbuypx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gyogdamdp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gefclfdbm.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gtipnfvig.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gwxixgiys.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gqxxigjql.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gytxmenex.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gaetlqmcv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/gluzfvwmq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/glcrphjcu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gbatawgvj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gvjawuulm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/ghayemhgg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gmrjmjqgf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gtlckrrsl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/ggcouivlx.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gexrybpeb.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/guvzjywth.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gorfemksg.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gaycovafb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gtulnupxj.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gfgdqpcky.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gpzcxljde.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gppkttgel.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/ggapdmqoe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gzsbviuca.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gylkgtcfy.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gytqvjsmw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/guaupxybt.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gpntpncbi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gqduzelzn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gkcrrefjt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gowgoxuqa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/guyqbbqxw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gplrqnyjp.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gwothoztu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gdddokyfz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjoqbqxaw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gwjladadh.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gnwafpznr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/giyofxjvt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gwikoajoi.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gjfdwmhkk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gboifavcg.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gngwjvlss.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gzxxbarqw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gtatdskbd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gfmvdefye.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gxaczbtlu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gitmvokhm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gjdfndpfu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gnuvwtzbu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gdrjvkvwu.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gqntjzowp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gogaalajy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gahaehphw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gbvjbkzfk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gmmgyiomd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gutozcugo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gygkqbxus.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/grmqyxvon.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/geqtmktdg.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gtjxdjldr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gudapqujs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gllsbvspw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gafggfgdy.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gpedjwjoy.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gadbyqkqq.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gsmybldar.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gchdxhcjo.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gincgufum.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gqfuoqohb.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gnszydoeo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gkpfpupzb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gmwruiyuk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gnbjqorjc.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gomgohkzr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gbshrwkkq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gzrmifyos.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gtehxnfor.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gpzbbwkuh.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/glcbhqwae.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gduamivit.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gpeouhoht.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gaslwbkrf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/grhuiczid.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gpmocgjog.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gqccjncrk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/govqdelno.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gywjceats.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gbjpqortn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gdzgbxgnu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gwgespygm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/glamivahf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gtdzuvduc.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/givvdghjj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gdjlfqwqu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/glkxxmijc.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gdoplakzh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/ghoxvcblg.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gyvawudas.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gjbydkdzz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gmgcqejav.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gujytjuea.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gaxcbbfwl.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gzrwezuiw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gmvxihjlt.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gqagtxlsv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gvglhpwtd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gxankizlt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gmtjbqlvr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/ghnmbvvjf.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gsgjmlxtg.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gchmzefnt.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gavuhxjxz.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gmvjcmoxz.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gsfxcucfn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gbkwtizax.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gvygfkdxe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/givctkbtn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gtkqzbmfb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gwdbggtao.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gebvhgeaq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/goeggxjdr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gtxouucyj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggdpochir.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gnjhouurx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyygoxnse.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gynlezesf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gosnmmqhk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gnhmmnmra.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gnouqrwgz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gdbbzycme.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gwujchszf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gvtwfxdtl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gmosurhpo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gbandcker.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/ggogoynmr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gejcoajth.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gzgplhbvk.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gpcerwvbd.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gavwiatio.sHtML


<!-- 参考信息 -->