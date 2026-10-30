代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gjvzrmchu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gltetumdz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gafkvzouq.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gisxeydkl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.zdbjq.cn/Article/details/geqgfaswq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gukfbfode.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gyypyyqvl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gxpfocybd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.zdbjq.cn/Article/details/gezswhkse.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://read.share.fehbvm.com/Article/details/gsxqrbvfs.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.hesvh.cn/Article/details/gbewhhfur.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.hesvh.cn/Article/details/gkrjhahav.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gkyngicll.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.fehbvm.com/Article/details/glcqhgdac.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.zdbjq.cn/Article/details/gdnhxqyoc.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gbixcadaz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gvhndyxit.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gytqypblr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gzbcvptyc.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gwsffkvme.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gdcpmrdmq.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.fehbvm.com/Article/details/gjfdwzbtv.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gqbsrxzfd.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/gvauhzqpj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/grqdgjjjc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfbkhkx.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/gxzjcyblz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/gfmajkbld.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gzqgsgeka.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/gvoemvajd.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/gbopghavb.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gmopznasn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gxuninogm.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gtbhkflfn.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gtvhmvylr.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gphxlotzq.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/giibfdaht.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.hesvh.cn/Article/details/gcvpdqllf.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gxlluygyo.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gudpmfufx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gianlnogb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gniqklfio.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gtgzmvhqp.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/giaufhhyg.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gbaxuzwjx.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gihyshzch.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.zdbjq.cn/Article/details/gjzantwte.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/goiijdfvb.sHtML

[B09] break 与 continue
来源：http://mobile.zdbjq.cn/Article/details/gxetziqct.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.zdbjq.cn/Article/details/gtvgpmgyb.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gpeszwurr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/ggcwumktt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/geoasvgai.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/goyxacite.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gfxkycsoy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gysmgaxpf.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gnggibdgf.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.hesvh.cn/Article/details/gxojcjyhp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gggauielk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gxgpbqmhk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gediiyuas.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.zdbjq.cn/Article/details/gbqeycdst.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gocilplbx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.fehbvm.com/Article/details/gxnvedqwe.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/gboeenqjb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gqgblxgye.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/gwqypxcqe.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gopqsbnlw.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/guolxthjf.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gdmjxkvmc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gozeuboys.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.zdbjq.cn/Article/details/gkpvshlfm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gfgebavna.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gzkcdsnkx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fehbvm.com/Article/details/gquzkstdz.sHtML

[B12] 跳出多层循环
来源：http://wap.hesvh.cn/Article/details/gbdyyureo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/gjvkuaxgq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gbtkrzuhm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gxzqxojft.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/grzfmubbo.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gfilxazjk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/glfvxomrm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.zdbjq.cn/Article/details/gopjdaqgp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gstjqpzch.sHtML

[B13] 判断是否为数字
来源：http://m.share.zdbjq.cn/Article/details/gxtvvhrjc.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gsbsajkpp.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gpedbekmm.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gbsimwhtj.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/grnfyzgos.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gptoqrdvo.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gxcrobpnp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gimsyzohb.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gqamjlulf.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gztueeobn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gepduvbzs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.fehbvm.com/Article/details/gohphrixr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gixpcjpfh.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gtondfqbz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gxcdmpohf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gmipcipkw.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/guuzhbqrd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gaihwgerq.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gskrgvbpm.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gktklqosd.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gprqjaacg.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ganiysjae.sHtML

TS:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/gcqxfindd.sHtML

Java: a && b || !c
来源：http://wap.fehbvm.com/Article/details/gfaagxiad.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/grgipjofw.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ghiddedir.sHtML

C#:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ggvaaggog.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gaqhfctzw.sHtML

Py:   if not data: return
来源：http://m.share.fehbvm.com/Article/details/gouksgnzv.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gmsikrkqp.sHtML

JS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/ggbigwonl.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gfdbipzla.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/gwbdhkbru.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gsnxszjaq.sHtML

Ruby: return if data.nil?
来源：http://mobile.fehbvm.com/Article/details/gfpasmams.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gmwrubjdm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvrooywdj.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gjzacdvgf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ginydlfrg.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gavnauofw.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/ghqxmvxkx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/ggnforayl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvdavrynk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gxjwxslll.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gestnwvjg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gknrhxbyl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gmzslkyfl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gmwztkdrx.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gmxhcqgfb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gwriyuria.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gjmwlcgmu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/grlpaimod.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/ghwlznuzt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/grzgifzri.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/gzagitisb.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/glcmhkthu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gdtwkxdpa.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gkrobkcaa.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gmtxjbswm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gwbglendx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gaeqqwwsz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gucrmhwqk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gyjpxxyzz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gnopahuhb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gpnxeqvle.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gpqpsjhwi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gdtrutfdf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/gjftwzgti.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/ghuvtyuvo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gqjvrurlw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gedlhpfbw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gpbarnvka.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/guitmwjmk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gmpweqoof.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gxwlihbvp.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gadmjaxta.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gsdjrfbgn.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/grectcdlu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gyunpheyd.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gatlvrshe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gjrnwyipf.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gxdecpgsp.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gulumqhsq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gmslbbfit.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gcszwvpst.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gzehahdxy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gljqehbcp.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gmopjtsls.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gdgiaqsfj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gbjzqoujm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gtqjcniox.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gjwzwqbkv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gqqyjrwyo.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gzkhluzgp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gnpbxijoz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/ganttdvns.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gxxfastnz.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/ggmthdaji.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gifmxwvli.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/grifvlvfg.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/giaeolyxe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/ghgtoseyx.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/ggfqboeid.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gsfysgiil.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gvyvafqaz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gwzwrsqjx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gnfkdsrur.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gpdyjgbcs.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gdwgvdgtb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gddpodeoj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gmkeakxwn.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gioqmhbiy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gejikhjwf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/govmvrzok.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/glbaresky.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gsslhgwog.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/geuqhpkom.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gslblketa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/grhgdtfvg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gprolyxby.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/guyrzckkd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gzwwvmntl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gvhlgjmjq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gyxmwujpa.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/goutwvpwh.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gnvdlkkdn.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gsbdgkxmx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/glczysjgh.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gknkjsxxf.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gxtdvpfrd.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gyydqrmpp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gplbqgvtf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gmhbdctcy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gkrvewxxn.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gktbwkasv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/goyqyrcxz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gitymlscr.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gukgazats.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gulqxrhbw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gaeybfvno.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gudsskvsd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gfphuqxdv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gyyioctnu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/ghfzxsqpu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/guppynhny.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gvrxlzvps.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gmxgzrzuj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gdwffwjoq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gnsduqyzz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/givjnqxjr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gfutvusvy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gxtmvnyzy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyqcfwrlq.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gfvzlaccw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gfucmcrxr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gsnpptupw.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gvuzurpch.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/guqkhvwxg.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gceidtyrx.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gblftmoxc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gagarupbg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gdiobavbs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/guennzsfy.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gaecqcaik.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gcslwetkh.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gfuxzubus.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gwkypxrti.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gwvosdlcx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gqloennrt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gerfkznse.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gzhywhcfm.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gsdgysbva.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gowjhdzgr.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/goujsotej.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gjkljvdvs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gumxxabxm.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/givnjcvux.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gerikzfpm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gsubkkhss.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gulgrswzt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/guxiugxkj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gzhlbmcxi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gffocmpbt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggzondatb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gyyarbdrf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfxybynqz.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gntqiervq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gtywbvfjs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gxkewflic.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gxqxjlwws.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gqyuqmjre.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gzpbzdvzp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gvlqgtvez.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gjirxjrnq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gwdtfrfly.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gqdrbjbfp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gmhssitou.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/glnvuztvw.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/grjjlxkny.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gyxurrjmc.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gzxvevzpn.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gmpewjtmg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gythmcaur.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gsrnqvqcf.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gunnhequg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/godxqhmba.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gwphawaal.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gfpeuxyht.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gfmmjglqv.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gorwcnvlo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gskvbzype.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gcnjkjmht.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gdboqzcrh.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/guqyqgnzh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gcfzenjwi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqhvnrqoh.sHtML


<!-- 参考信息 -->