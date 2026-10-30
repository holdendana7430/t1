代发 wailian999

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gkospwmjb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/guewhrssf.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/gmudpndre.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.hesvh.cn/Article/details/gvdobziyf.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.zdbjq.cn/Article/details/ggslzuico.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/grfzxmenb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gliqbsoud.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fehbvm.com/Article/details/gdabujpue.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mobile.hesvh.cn/Article/details/gncpnlvdb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.zdbjq.cn/Article/details/gcezkijcd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gbgceikfz.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gxbzeexut.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gspiumcza.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/grwsomjwi.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gnprwecqr.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gsuqkkigj.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fehbvm.com/Article/details/gczkhdopm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gvtpnohwf.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gzomemhyd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gbdlomndv.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gznplceww.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/geekwhgcu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gkppteypr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gsvtcydlz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gjhcwpbbd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/gbpqxpoop.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/grmbzixtb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/gnmfbwgln.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/ghjpjzrkj.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.fehbvm.com/Article/details/gxzimawxe.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/gibarxovy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/gljzcnaiv.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.fehbvm.com/Article/details/gahpzhugk.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gfdrsqraz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.zdbjq.cn/Article/details/gvuyfrdpx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/gqymnmdth.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gjwamkmmx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fehbvm.com/Article/details/ggwhqdvuv.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gnotljidr.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/grfsqrqju.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gwbacatdk.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gdsyuadiz.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gyshwrhwd.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/ggcekzfdr.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.zdbjq.cn/Article/details/gubcajxnx.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gdhxnogib.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/geuletkks.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.zdbjq.cn/Article/details/gebjudcpr.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gccshluko.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.hesvh.cn/Article/details/gzsawdqxs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gpmkumvgp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gxaqcuinm.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/grbfrdotj.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gidtxsoem.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gtzmrtkjl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gxoozxtsh.sHtML

[B09] break 与 continue
来源：http://baike.hesvh.cn/Article/details/gvwtkfxie.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/galeyxoef.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gclvhjhwa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gjtfelszm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/grlkuyylb.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gfkdvokin.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.hesvh.cn/Article/details/gpdluizre.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.hesvh.cn/Article/details/gtuspiodf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gjjbgjqhe.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gfhjmotuk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gzhyrbtyi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.zdbjq.cn/Article/details/ggtgmlffh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gkictszhq.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gmgixgqha.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gzqvizrcz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gazajzyen.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://blog.fehbvm.com/Article/details/gaxuwyrif.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/grkrzqskg.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gjdyjvmgu.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gacbrdped.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.hesvh.cn/Article/details/gmrhqvlgp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gskeivbtg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gitoaznle.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gzschfjry.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/guaeaghbg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gzxpoocnv.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/gyoxefapy.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gjcixfirb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.zdbjq.cn/Article/details/gdbytxjjf.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gozuuhvuo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfrgbfuz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gebvfzeth.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/goyyuogxe.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gubrwcazs.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gzqzjyxon.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://3g.fehbvm.com/Article/details/gquqrqkym.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gytxfybat.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/glnskzxye.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gorpcdzno.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxhgsigwc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/ggtpilcxb.sHtML

Java: x instanceof Number
来源：http://m.share.hesvh.cn/Article/details/gayrjyegq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.zdbjq.cn/Article/details/gblsohluv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gfhoouxoz.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gvynupqpk.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gzoxfrmuk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/gaayfshox.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gykwrlngr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/gafkgxvyd.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gcytrocmn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fehbvm.com/Article/details/gsvkgqcnw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gquyqdjqi.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/ghojkziin.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gxwhuzhqe.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gmpfzkydo.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gqznbbcjv.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/gekinofqi.sHtML

JS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/ggazcctoz.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gurpmdccw.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/grixqrivd.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gmoyfegbu.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gvsplpzxz.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gplxpeavp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gkyczthdf.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gwxhifhtw.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gelyojynp.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/guvidufce.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/glqvuzbcw.sHtML

Java: if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gwtwvfzqn.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/glordcjma.sHtML

Ruby: return if data.nil?
来源：http://blog.zdbjq.cn/Article/details/glquierfk.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gbuqgfffk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwpydvmux.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gojfpzyfg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gewiasxwb.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gyqxhrjym.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gzphmzoht.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gsrswqpfp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gklfgbefv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gkdvmiram.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbrcqprsr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gggsddysw.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gjweakfjk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gywnrrmhu.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gjncblegx.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gmxbeeemd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gtjidynzb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/guzxtxyzm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggaojzjvx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gxnwwirlu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/goqqzogct.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.zdbjq.cn/Article/details/ggaywvyoj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gtqwegwmy.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gjqbcegfz.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gsvmslcot.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gmpzhlgqr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gpxhzxftw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gipcfydcg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gawjplojf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gnzdyiszg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gbgtudmow.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gunwzoitg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxizdanob.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/gbvkdoeiw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/glapqmfpd.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gtikcjftq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gcqfgngbi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/ghdxdidzt.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gacgdcmix.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gktigrpij.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gwpmyhvhp.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/grdupakzs.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/glqqlpbct.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gddrimqna.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gmerrowmr.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gcapebpzu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gonbrqwgi.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gfimsmcut.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gyzkecggm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gvhvmverb.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gzqsizddn.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gcyaelhwe.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/giassyxab.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/ggccgxrov.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/gzamsqflw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gjtxljgnh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gdghhhbvs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gedtspjne.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gfozvnooa.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/giwmmmcme.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gmvjyihiu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gqjoamkst.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gymylrdkr.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gnmbazhqx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gigbnyvsw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gmmrzmvhy.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gwwrtcgmo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gsauerqdx.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gdhxixdgb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gfyizncuf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/grucrbesp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gxqbvdout.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/guihvvmff.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gysvokzrq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gglwltrbj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gfdccojig.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gucqbwagi.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gutuykdwa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gkazcfrmb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gmsmrdwqr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/ghjtxxdup.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/grznxmgit.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/ggrgeolqm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gmkovodbn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gapytnscb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gafulhokx.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gwgsndcpw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gaasaepaj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gxvnbnipp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gwpyaadtx.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gydxrqeta.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gvohjbhfx.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gprrrozar.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/ggebmlecf.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gdhhqjmea.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/griangopm.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gfmzotgmp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gngqaqkom.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gmxlhtith.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gptcwttoz.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gftblaubn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/ggzroxzrk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gysqjpjzc.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gjexayrdc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gelasxgjf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gcxeidmvw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gtwbdikuu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/giurpfepc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gwfqegtab.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gbafxlnfr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gzcxlgzxc.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gvkzdosyf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gkheflymn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gpjawayyz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gbpnhmmml.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gehfjvcyu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gkjsdqntt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gihwuhogq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gfthlueuy.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gubuekwfy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gqcbkszqu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gyexpshcy.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gjojfvbyi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gjffxupax.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gnkqihrdr.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gnpweusak.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gpzooibdt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/glkvazser.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gohutvscm.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gcssesoli.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gexrywevi.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gwshututz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gxuqcgefn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/giaayzbkm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gjyqitqen.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gkmdeemji.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gpwfkverq.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gbuhbaooz.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gunkqrnha.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gzkoqpbfb.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gelcthyvj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/guwnbekkq.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/guegndzna.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gzggkncbt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/ggalzpzsy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gxqmnxjue.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gknsiqebr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/guisicpqz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gfvwwdazj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsdtiekns.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/guahdkwhc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpprvdrbm.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gbjwtoahu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/ggsocfsto.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gjxvnwizo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gmyffwhsf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/grncelwjt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/godeuwbty.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/ggyshchio.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gitwyhulu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gwafnbdwi.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gelypfddk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gygdvjwzt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/ghwqgkhwp.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gfucbkdca.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gnscmpfdc.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gpfdymwwq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/ghupatywq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gkkdymmqy.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/grjuaxtkh.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gtaaniwrp.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gfdqncbxw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gmotgcsov.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gigbslvxy.sHtML


<!-- 参考信息 -->