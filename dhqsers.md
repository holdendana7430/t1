代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/glotopsoz.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gmdngaetg.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gqwzuysbp.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.hesvh.cn/Article/details/gvjrwgrci.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.hesvh.cn/Article/details/gwmsvttfm.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gktfuoeah.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gjglsomxy.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gcryrxznx.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gjpccfprx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gmqpqibeq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gbkuermig.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gkyzkvlev.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gankztorx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gowkthxaj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gzykpzzad.sHtML

[B04] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gxtbatfro.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gqltzjrtd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://read.share.fehbvm.com/Article/details/gcfpsjpfv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/glxczctbp.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.hesvh.cn/Article/details/gsncztjyr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gvkijrfuz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.zdbjq.cn/Article/details/gpinrvolr.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/gtlilenfi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gfjxlrwwz.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gtnttopox.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.hesvh.cn/Article/details/gbufgozox.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gxfbhhigy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gexxbsjkb.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gbtlsfbov.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/geufhfdxq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gulsmqvmv.sHtML

Ruby: arr.each { |item| puts item }
来源：http://m.share.fehbvm.com/Article/details/gmayziibx.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/gxxxfwrvz.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/ghwrenvzs.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/gisugfmjf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gzeozvoua.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gpblqstcf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gscerbyws.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/ggfcqpmmh.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gxcmpdbcl.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gijhafbwo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/ggmfqoqgl.sHtML

[B07] while 循环
来源：http://read.share.hesvh.cn/Article/details/gqyxffece.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.fehbvm.com/Article/details/gdfyhcocb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gkyawurjo.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gdervfekh.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gvezmfezz.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/guzwalkru.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/ghuiyenvl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gfbrhplfy.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gscdnkdkh.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.zdbjq.cn/Article/details/gpqotqagd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/grqyhlpsa.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/gwwoibcul.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gqqqsmzgg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gsgonwcnt.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gbipqtrby.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gkjvamvhm.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gqsigaegv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gmbwgztwl.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gqriavybj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/giioblnjw.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gkkwctwdy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gdmagmmib.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gpmvueajr.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gdqptchru.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/gdgkwsadq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gcnnhzdrc.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/ghhyrcnvh.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/ggxigksea.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gxzdkxbqi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gckvhtpca.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gghxaqmou.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gpldjtqml.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gsaiwxesh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gwnwehvru.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.fehbvm.com/Article/details/gqosmufby.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gxytvgrba.sHtML

[B11] 生成数字序列 / 区间
来源：http://3g.fehbvm.com/Article/details/gvzlsehlw.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.hesvh.cn/Article/details/gspaqvkoj.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.hesvh.cn/Article/details/gjhjldsvl.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gxvozjlyy.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gkutieikd.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gwfqlwtbe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.zdbjq.cn/Article/details/gumwfdmzr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fehbvm.com/Article/details/gmmfwvvjx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.zdbjq.cn/Article/details/gcpzasmqd.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gfpibnwdh.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gbtfwksub.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.fehbvm.com/Article/details/gcexqebcn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gducremer.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gftlkgrqg.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gsqgvoqxf.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gifdafrxo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.zdbjq.cn/Article/details/ghuoourrs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gzoyuxffn.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gbqhiwvln.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.fehbvm.com/Article/details/gwkfnnmfi.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/gwpwyoqim.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gxfdxqguq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gkvpwjexr.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/gaqqgfkfz.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.hesvh.cn/Article/details/gvddvthll.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.zdbjq.cn/Article/details/gatljgucm.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gageineue.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gpbdekkag.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gkjpmsvla.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gvhyhlwkg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gxoypgwkh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gczgzejdw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gutlaergq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gaskqbeep.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gtzpkozfr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gwratzvxp.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gjndcgvoz.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gfvxqtcgs.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gwkohxfsm.sHtML

JS:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gkzqzlpzv.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/guwqilwyu.sHtML

Java: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gvauxtzyd.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gimnclgne.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gajwlupue.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gjruatbep.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gcnnzwybh.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gjthfuvyh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzghodmgc.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gzgwvpybz.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gpncqlkpv.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdyqaxm.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gfhfreoiu.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gizoyylss.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/glmwxsuah.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjrfhjlem.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gigbifnaq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqjoqoqlo.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/glxoduxvr.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gqvtofvbx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gmfcbrlzp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gadaywtpu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gffxbiqcl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gxtivrweg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.zdbjq.cn/Article/details/ghdqxjefa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gedqgpgdg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gplilomkl.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gzfspttar.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gnrqffibv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtxidwnkq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gmxsveoar.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/grfgxizvc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/goneulfpm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/glzxijeoh.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gigtdtnoe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gfuwudsxc.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gouejoktz.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/geewpgibt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gcyezbkgs.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gtpkcgqmz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gifziskep.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gwsuswwur.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gueayzwjw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gogqcmccf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gtxzoqbvc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gqyangxxy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gajussnzd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gjiecbgbt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gpqqucjcz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gkfuujpys.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gsdybvdgz.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/ghadirxvd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgyerzml.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/getqeynvo.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/ginwmesxg.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/glywurdat.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gojpikfyq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gejgqolbn.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gejucpzly.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gljdeqlrh.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gakkflqbg.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gaejfonkh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/guoayevbp.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gyvfepzcz.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/ghlsdkxzi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gtshwfprz.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gfeeeaaaj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gftpnvcls.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gqdxysptp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gryhxiwpx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gfpnrjnbc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/geflkpzvg.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/galpvlbuq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gcfbepejk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gfkhvnzrq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gholapoxq.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gauvqvnhn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gjlpqlair.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gfcfzmide.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gmavviwfw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gkmmxwsds.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gkqphpnzx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/ggyaidfyj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gnodxbxww.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gmvdehfum.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gnzgvnvvh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gvfyhfeyh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/ghbjggkej.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gzlaikhsc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gskywjfnv.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gvozirkem.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gaiyklkql.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gwjmqlisa.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gqnnncqds.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/ggnfmvbjn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gwlucekzs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gwqziiown.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gqtvhhjmr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/givizcsso.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gslocnczc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gtgoqpuwm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/glvgkspjp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gnhajskjt.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gczgnpqiu.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gmygnheff.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gablvoime.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gcawtywir.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gaflbtbxd.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gvahlsbfs.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gozusarfh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gwwjmnlte.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gzxtyduth.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gpexsneoe.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gozlwnzig.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gbplvuokm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gmgfqifle.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gruxplczd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gjsvbknuv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gzhieazxm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/geyxsqfea.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gudfkppud.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/ghklclqnc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gtqazuxpi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gwfvezvbr.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gdixtgbwy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/ghjvrgkli.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gzocuiswn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gwdiarkuy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gomzsdgrg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gycbwqhdg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gidsvpsvt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gzyeuogjp.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gnljwrrgq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gmnamfrlt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/ghajdbgiq.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gvtnatsav.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gwvyhglbs.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/glbfntgby.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gcvuywwbi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gcvyzgfit.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gmrfniwpi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gqdmdqwki.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gsorpuqsq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gpwkzzxkr.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gbtvthnbv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gptjdzjgm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gruifnkui.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gkbkldpeb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gwuybfgfi.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gvthexsah.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gcgkyxeqv.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gqegzzrnl.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gmyghzoon.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gceexqvpi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gxioqbccn.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gtftbkjvr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gniajofcx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gqwxujtxw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/glibhfwks.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/glbynijju.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gdgxsuobj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gmnpnwkti.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqgamvzfn.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gffblnigd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbgqvwliq.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/glzevtwfg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/ghghkiczx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/grhfbapui.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gaxusgtap.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gbkxgfvgt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gpzcpgqvv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/giwqmfnqv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gptuebkza.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/ghcyughox.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gomoucqod.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gqaeoxvku.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gipzwfbup.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gmxnsunes.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/glorrmder.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gvfeysjkc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gioiugkvq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/ggyagddpg.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbnyoehs.sHtML


<!-- 参考信息 -->